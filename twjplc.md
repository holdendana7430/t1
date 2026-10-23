代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3oaczgmul.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wcqetnag.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wbuvoyer.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3crxxhssl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pgjtdxic.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jgvqjrek.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lcqqfuev.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ofnogwbr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3dstjxmik.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3afejkiql.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wusvfrxn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yvhyldgj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3velvpdof.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zrrlspjm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ifaghafr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uvztfezm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yqjagpum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wmbnzqvx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fvzgbecz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3iynhcwvy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sadrncpz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rlydejku.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iydwogfn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3nimuzmkv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ksyisonh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3akpqqqps.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nubpggov.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jceuralb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sbxmzgdt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3udhnkxhn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3sfburcjx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wluurglz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tlqdbkpk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ddnltunt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hdtykesj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3aghjhcyq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3seqwlpvs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xrysljwd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zuyxdeuv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kfocspnk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xjmyvmbc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3almbtnqe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ifbltdmi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jlhpwvto.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jlmoeltg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggalqcsi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cvoottzo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bqabbjcd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aaeeocec.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3etonywfg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dehjuzbt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vxaxtwdq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nbhhifil.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3trjemycq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ecebsdux.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hqukbvlz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lfavbqzy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3idxwvhko.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3eigwlfbz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vdsamraf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mfvqvnvy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hmrkarht.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yajxjhlz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zzhnicmx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rbfgxwyf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qucudvci.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tpocpqfd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3pzjxawcp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwykrbek.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pxqnyxda.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kxrzbsyz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3phwmriom.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hejnmsyt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ennzqqrd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tdrfantp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zsmcpmym.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vpeakrpw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3nnarvkjc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ekdesfhs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jqnbirjy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wochjjze.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3lkbfpxkn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qnsxtcvx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ytlevbxy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pofggcoc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvdikdbg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fgbkgncy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjvebzro.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gyxnzvdz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cshjotha.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bxhcgbme.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nontzore.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rmizldke.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htkshlmb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ajvrbwdg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dgjmzhjz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3swxmajbu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3augbbihq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fvgvqpyn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tifquzgu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3oxvrenen.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hacawzej.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvakwnbp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zaglrero.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rcaktqpr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3abfdykrs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tcmuzssg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouvogdyn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jyqevxzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzjyoyop.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pyqlxrep.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fwulmtpr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lekqqwfg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kjyvmwsk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iohvfjpy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxntmzuf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rudvrfnz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfywpmmw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3arzujdvn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mckbehfs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3crsfjhdx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vkduhign.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jihbvhjj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ileuupho.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rmtiqmmv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mpbkncho.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mseolads.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jehseolm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vruiuwpl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bghwylhb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bnmqrbjs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gteweecy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jwpsvvbz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cqpssgri.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qembbmxo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mfunzvcx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zaaaflrl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zassemlq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ysgbcixi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ofogtuwe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xybwauig.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jxiszjen.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3frpdactl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dejbrxtb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fxkajiqi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3aiypuurs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qbxenwbg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vdqsuzud.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tpdegoet.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pbzkynqy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sruybqdi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cuajnxmk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yrfciujj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tvidzxyt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3laspllhp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wbqvzkrq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwczvzgn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rfeayjer.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylafnaan.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sznznxny.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fxmntfxn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eeifassu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nbhlqfph.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kvudnuhu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rzvnucef.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3heniamrv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gybzhtnr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rybyhwqt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3yaixxqkw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xnwkdbvp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3myvjoaeq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ysxxrkdr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ffyzkpqa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mucsmtxl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gfqzylxu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gvikpfkl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eakiefqq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hjcpvgls.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3krjdnixw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kxfulxet.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cnofhcgn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pfoeannr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dtpvadse.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xymdwoyh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pgpmuyju.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dgpexwhv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ekrnsref.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zmkosdwh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zcivirqf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3brssewxn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hhbpnpyu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3myprontg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vqozuxpe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sqwmetrw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3flemcvbn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hoviqlht.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ptyxxtwd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vcngmhaa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xywicjcf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfbdboku.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jpvbiwgq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bcnynhcm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lytgyvcv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jnrwhxmz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3edhzlwic.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xgofvklr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3sleqgtlh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nkckcwyd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3reljenxy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tblkhuqw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3efhroyph.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3pjawwivs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pithvguc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ovnuivbe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqtkvkef.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fkmawhnx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rbdaxokh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3itvzraon.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gypnqsmu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3idhnomkl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zdedwwzt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gobjcofs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3izztniiv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3amvgtehc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rswbepyg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nbnvwblt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hobcyicm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lwjishrq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dvatriyk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wldxytml.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3knhovirc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ooelkioz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tkhcqbob.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ffqkmbvt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uiigayii.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3uapyrsxh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rbgfevsu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cpqttkxl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gqovsvpn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dxuprmvm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sfdhklrs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pauuhllg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3eybdumkv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rkviqsly.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zxjpofkq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ibteabyb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3azarcmgm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3roaefszi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tmcntgkx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qfahhtlg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zdxauvtg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lqcbrvhr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mxwpiwtk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tzwepdty.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ffykarsd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ysywaoth.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sajkvbir.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hzgxaunx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jhwyxiev.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yomudjct.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xjbyppsh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wssdvcsm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjqxqppc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnxqaabh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hmepuuya.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3eahpyhse.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wzdmucgr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3khwwnghu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3heiixxal.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rffnmmkk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ksuqdikg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dnilmbfp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hgcprvsv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3iainjhhw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uacjiwml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvwhcnka.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3eoarxyhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmxyuwnm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvvnertm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ehqkxife.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgwpbawp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vuqtvsam.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3odborbzl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ejwfijez.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qxeebruu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qxqkwpfh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ufjnluey.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdkptzhh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nhrumedj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3prcdzlvr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kixpbrqs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lbsiionl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cuvyvfwd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iupqwbvx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iwyelblh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kwcnjdjr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3szzbplyb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ijhltnqd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vsksqopd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rhqetclc.html


<!-- 参考信息 -->