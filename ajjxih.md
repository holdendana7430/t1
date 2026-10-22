代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2yjalglyb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ixamgkgh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wcirizdo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zkwwlyvu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hbcbuaou.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ehdlehgh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bwucdvom.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2flvwthpa.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2legnhoff.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oruyhqca.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2thvctnan.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zgfcgaxz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gqegmnyi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qdpwhsug.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2puzxokxk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ovfanyji.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2chzeypqn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jbonbqjj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kelulmem.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wswguvua.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wkuuankr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jncpedvt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nrurtcwc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wgrytdvh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lwmmrpkt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xvvsufrl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qulxofvc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2eprxgajl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xnefpfjm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2grmnohfc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kryoimlt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2umnfgqkz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uzkbtllb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lplgszqh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wiupcfsi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fjojrzpj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2djawbiwt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ojammgce.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vvmcskhg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vgbdvhcx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzmjcftm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kwnoqzkm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dpzoscvp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sffhfyxj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lykzlszy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ywbydnwa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gbevjupt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wshnmnuz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xtlihrkk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dccpedte.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2uchwrril.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vlswptoa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lthebknn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rzqguedc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pdqfenjp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xvjrzzgj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cqctxjyl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sirrpijy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2usrzlxru.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bgowlyee.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yizensjp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfhpox.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yzyopmsl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xfyqaqlz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ongxvgqi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gfieyoxw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ogosmthb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ayozogon.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uaggcxpv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wqwebeti.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zwcashbf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nodiwcqn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufmlnelv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2raffppxq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pqunovgo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2llbuhsur.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2thjminss.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vidagxlk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2itkojdea.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2aydglpfb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lehcmwvi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kaonobza.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2adhofiey.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2diyahhei.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kkstogww.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cgdazdnd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fwefvkaq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2upmqtahj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ekiebdma.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urzktrso.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qxhaeeec.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wcwqnwok.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wizeotqz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdzcudsh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jtsryqed.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chxkhrvg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wzxkqlny.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ebogvovm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kcmagmes.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vifycumj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wrxpjdtw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wmwrtznh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxkydz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zcedkibn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kumpqvtl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mmblujnt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afxfchdm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hgrzlvva.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mtiuozkf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ytrzfmsl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2aoozzral.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raoodxgw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ryjbgdoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxhfdzcr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xbpytvtd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xbdjvwcn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2pbwtamiq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pursokos.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yuxzaydn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2znlhctds.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2llelgnrz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hjzspeco.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qktvpbwv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nreuhhbd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrwnrnuu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vctmtsju.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxuvnsez.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmzmvugy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2akrhsvio.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2soujkeab.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ilpopqxe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2snelznmf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2onraseql.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zobhtqmw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2prajfzed.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dffhtsow.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ahcxokdv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wlmdpgjo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bxbuiafd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jjjqvavn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ajpmorml.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2agsukbgs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mcftbtbi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hokkeomx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lklvssug.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2srldkxgp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xznykqoy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuqybyzb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dzyvptha.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qgwuiyaw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2urmdsukf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ueuroijf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmwvtyof.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2iwdxknjx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nxtolagw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dholmosb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fosbykcv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uarsekfo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qlcfcpgw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hauacvuq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qsyoladh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ezokfnjs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tfmaafjp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2srufabyv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jqhsdrxg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qvsmokkr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmvpatjd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kvazdqhs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sytjccse.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fspsmsei.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2byvvsnbr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dptmgdmh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2trpfvird.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tomvtfxk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2effzzirh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2piorxtnn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ttouncdt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhnyaaoh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vwexulvi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2opwjubxb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqbtagw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jkvsewbq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcltvevz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pxlabzvo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2exfdkple.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cxadbmxx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tzodfpgj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qulkfums.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2svgjmory.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2arlhhety.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yoyvbfyz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jlislukc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2chpschyk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2rmufmqbr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2yvcpmglb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2clkwoouj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yvqyutmm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2brkfiggz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2njghfird.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hphzlhjx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cwklletv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qghthblp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mddnruus.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2iqyjipxy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lvbjwshm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pezcnvwj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cgthchpy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vxokdfbn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dsgjqamd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ptolhnqi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gkfxvsnn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rtmfugrt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pcqbhvhd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gswdlxiv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2grjcobkz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vzsojkcx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qlcdmibb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tfyrtpva.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2igqixmal.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2knrvfxee.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hqdjullr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cknqzupu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vjvqhlhf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zehqcgki.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rozummgr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2foddfozr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxfgsnab.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wipjmtzi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2icmvjxrg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kzciplox.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2oldwgdhj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xrjeygig.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wirrxzki.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxlspjhf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xzqsupav.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cirlrvig.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ywcuphys.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rauglepe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2owmjlnii.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hlknxngz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nwgjinkd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfjbeqjj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2setylrpa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bztlduxq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2osarvkay.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2txcbtzjm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yjedwted.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2htdcwhvw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qcvcjswm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ewfhjfmf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gfcykgum.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sttahoaw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xklmngpf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2koavijvw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfubncur.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eogxcmfm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nhvmqtwf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jpgjfwvy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yzhpicdb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iyceusxk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rdxsqbsa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2egzyzcyh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yanxkhvw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ymdxwauf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2chzudmey.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jddxomdp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cereaxjd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2awaubnrz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yytefppd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2peykisrc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zibximrc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2thliwhng.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mswmgppk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2popaptag.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cbunfruz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wnqiivth.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lysdhmus.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yygjdszc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ekyqkbof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nodixjbm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2drqvgkvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mffalcle.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2juanrevw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uzgblqei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cztiscxz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2iiprfgbu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2luucswfg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2volafhso.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ygyxcjok.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tvbclnzz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fsaslytu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pruyxhze.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dhlzlksl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fhazovyu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fiwmbobh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2soinctee.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jdahxgzh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lmhhkbfc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jsipokrw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yhvykrek.html


<!-- 参考信息 -->