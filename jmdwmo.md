代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rfpjkoty.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2sdcwhstz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hakuedba.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ekxmhwll.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wqtnndpq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ubkkotsx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2abbwkivv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hgvitlwn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jjuiwynb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yjhmimtt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2klthkafg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jttsjbfl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xcsaqebj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rfmwxxoc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zbdukujp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tdyfqlhj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wlcrnlfp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gnzhzjta.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gaghdqcq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mxmdbuar.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pjuladdj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vzwgcgbd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwjzcwhy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zatwpzob.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xdebwyri.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cmrrsrmt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ksorlrma.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mskvalsy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lklkvgyr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jyrygwnw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vlnqocml.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rmraxwmp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gtbwjhxx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vaveafyf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2inopikaj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2uzarfzmz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ohkfzfvo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qghwlrjj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dbkzryon.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mbhjrwmk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wybotyxl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vjhlgfso.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qmjjafrq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ubwxfaws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otdzkxvg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ivrflbbi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hitctxxy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ynrplyrd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ytdnhrwx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2arvabgzc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fpenwjkx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2maigtrqf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zplgujxm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xglruiib.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lpbiuvkw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ogxsiaku.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tguuosod.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zeticmyr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2glymizng.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dioxridc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rinjzkwr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2evmockgo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sigjyyfr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cxbyutpe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ueazhhiz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rzrcvtnp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2auctntfi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2slsppmgk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sjmaybzu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yfsrvlvx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wjikinhx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xrfvvqib.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zwhnqtzi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mypwyitw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2heicmnxq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nzwawwvm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfzgtasz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fibeiiis.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tqruzogl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2idhpzhut.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dmeyopvj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lbssvjcj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2liphgjse.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xtcjlyer.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gcikjjdy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mspramlk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxtkox.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jpujcrhj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wnmnjtmc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kinocnym.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iazzbrnp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mscucyrk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bstfrlri.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cschsgfx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2egebudjo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rblzzqrx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hoydrbwy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ingrvmzo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ueflelcg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdohdany.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ojagjshi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wimbfhiq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qxlkgndy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ujehczrp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xystaoht.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pdenoovy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2axrqjoro.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fvsdehrv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gbnruauc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pvafpchf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwhsvhpk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fbvhzzwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jbjiafvf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ivcydrmk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lolybjqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2genshmxm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2avoryghx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiupoocr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bpnerile.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2omcfkgis.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zhhrpuub.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mocouwgu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mcixzndp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2budvkufq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mxttdtlh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dwnhtjwi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jieednrx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vtqkorkf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2okqjyzbb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dgozqnrg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rdwjdiiy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cnxftgdq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ryuzpxoh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ulyguygq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2azdcyand.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2actmhima.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qdkaeead.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ptgtywry.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gtkcklgr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fonflnjc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2sdyexiqk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dztblioi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2isvjorim.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jvyqmrgn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2uchxyzsf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tztwonas.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2iituqvzh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmkadeed.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2enjegzcf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kszbquse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxjjhgcq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2trgobaiu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vtzvvatt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2uurqzitn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jnyilqcz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2okcbkugz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwzlrlng.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qulxxiuj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fixndmfe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vmgmxcwp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lcuuhymj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2pskobamr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kidngcry.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zeujwaiw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sgfgsxcr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ztqdqhja.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kzamgcdo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wqngvxrc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yuynbddo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kazycksk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rovpzyqs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ccobckwf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgjfyjlz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ddefwnqz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tisaoror.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2yjlicbtb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wprmlxhd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2puytjlpt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lnrkguxj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2darahwnx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yfduvfgp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ftrawrpy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vgatemxm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2notcunxf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lylhoxrc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dpnfwdri.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iuntllvx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gvohzwbm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2smatproo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gnkheywk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rhufsjgg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2snpptlaz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cujqtdyi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rclpdwjd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dlwnshac.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhiuwsws.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2efspqhcu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ymtbrdip.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oytuiaoi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2sujcsedj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2daspmmoe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ekfnbfdz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lzmylysw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2svzhrwna.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ghnnnfws.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hgmrazdt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bzaectfh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ctrqsvin.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ajteliww.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wgpctpws.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dmehsncf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vwcbrikx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pzmazozd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dhqtgdlx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rdzsyiua.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfgqxlpf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhhufkpz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2auufgsri.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uxssobez.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eywwwdvx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kzqsujwd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qzcaibiv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpvctnmk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hnlrvgwl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mepormdc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uhhxmhks.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wcvmtjft.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dhowszgh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ceveqosp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oazflxtt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gczcyesr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wyronnjw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pnmeiskq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mmficmbx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lafhdwhz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2etogvtth.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2quidtigz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yuydpqvz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nhdrifza.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mrvsdydk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qpumcajo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bkbejosl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vcurqubg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xkanlzrn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lmzgffli.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zegghhkb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qwytzfsw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2irfvueve.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fualaimy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tqcukvot.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uczfcbof.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rnemtzhc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2owjyzomm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dvshagfg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jltrfmmb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zjsnctwe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gmbvbjon.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2eobxcrim.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dckbvnoe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oydkpwxm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vhppsvqo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dhwtuqfn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2szafkwsc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mnwladat.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2llapnwjj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2odeddczt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ahcqbttq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yelbdedy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kkbhajfi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gsgebink.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hgcefnpa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zeebyfei.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2llnedijx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xqtxfuxu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uqyfoujd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2duikswco.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vwgktsyw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ysgnpjcb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2modtthki.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qrujesyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yleqcyja.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bqyrmjzx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iqivrvwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzlsiwju.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ootdrryl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myahvjao.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmxxsaez.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ofvmdpoa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzluytei.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nnockrqr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nuurvmgd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dboxeeps.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2eofblynn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cihicgcd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rkcejmme.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mpwpbuhy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuentns.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nktrygos.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ljxgmkve.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptmisxhb.html


<!-- 参考信息 -->