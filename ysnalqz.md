代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gekbatxdk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gwawrzltb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gurhzigsn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gjfyrkeud.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gwhxgbdph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/guokxtxlr.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/golbmxmph.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/globrqcwg.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gxekdqoyo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/goqjwpnxs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gqjhnvciy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gthenhviu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gsijddhzd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gxnqyldhm.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gttmacjta.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gxqbfaedz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gddaenxuw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gzmcsvchz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gelxzqefq.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gtpbpuquf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/glghuilif.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gidfvuxmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gclxamdgm.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gqzwaqvoe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gmvaftmxj.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gqcmbuykc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gkgwbafoz.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gwnezhvcj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gfttvqkvy.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/glbesxraq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gksbtchrs.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gxkdrphfi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gcqerurfl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gnvbahdfx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gysfuikpj.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gynlwljpc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyrptlfpu.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gtqrcxucj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gukosteuq.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/ggaqncoak.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmejyczbe.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gomptgase.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gdppgfphc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/getjyabot.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gprgxquha.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gffirvmfb.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gnovhbpjg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gwovgoixq.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gkucnctme.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/glacwinoe.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gqsrspvom.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gzrnzithi.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gpudfimci.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gqfmvkbqn.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gmjnfazan.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gmyksduam.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gwmcthnwr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gkqeopncd.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gumyjiwpu.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gbtbtnktw.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/ghqguvdps.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gtwfmgbdf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ghpxiggqx.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gcnfqfenm.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gkjniqhqe.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gmmambffr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gygjrdcln.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gyhnekjxf.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/geumzsfkm.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gdywoueiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/garldjgvx.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/ghqpmmmjj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gzjfobnim.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gkwawxlhe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gejmfixei.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gtiyvcgpx.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/ggivqbgoe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gvprjefmt.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gdjtcotoa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gzbtdqasq.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gobvkazdc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gzcpwcsqw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gsyagiyhm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ghlmgpivq.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gyfbsiyvi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvwjespvz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gvddlqguk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gkdyxxsoq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gnkdtlptf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/greqhdxpg.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqjvljoyb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjtubwfmn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gccunfhfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gshsqqeqq.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gphgzdbhl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtwbmlh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gmxuyqkco.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gtwqudkls.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gpnxncujm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/ggkjgrnhs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gtdqqxivn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gctpxhmer.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzwtlwydc.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gtmfqedno.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gmsadiqrg.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gtbiwhraz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gtooxkktk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxqzkejce.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gdhwwankm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaxhciuck.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gqspjpqtx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gpujwsjzq.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gvahrpvfo.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gapojyaxh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gneciuygh.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gmjbjudys.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gphdemtgn.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gccvlttml.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/goxxwhcwp.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gfubrmrei.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gcaiyavsp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gskxizvfy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gjbwjinnp.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gnbeazjns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gwzyvlqak.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gsyoprlol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gaxvbuxpo.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/glotibzlv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gutkzudzt.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gzqhkohzn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gaszbyuvt.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gbsmmitgp.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gtptthtyn.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtywzborb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gkujvgebg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/grjjcihxr.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gloyszatt.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gzzrfewql.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gdaimccrq.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gvtoivihd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gdivofwqf.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/geqxtatew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqdelitog.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gozchbesp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/grlwnhbcv.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/givjuhvqq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gyenqiuld.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gxzfbgtjr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gwdfofllj.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gpsshlxcf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/glzuytcth.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnqxjhcqe.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/guodprgid.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/giyomzkwk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/guoaiostz.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gcpgwsnsv.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/galykielj.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gwqdpcwrw.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/glhpbxtal.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gppjvynis.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gceajbegs.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gfbprzcmr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwphrgfbh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gjtmmhrdf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gmqhyilmc.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gftnumbte.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gigqhaqwm.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/guxfxygst.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gbiviqjdv.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gytilrfif.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/grzevrihw.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/geiihnrsx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gjdwqzqsv.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gmfsuboss.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gqggcdxrj.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/goajfkzrv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gupcjigtg.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gdokxqeie.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gmhktvryw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gkdnbheam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gfdaryvfp.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gfcaumdfp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gmukiijub.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gbkgqsexu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gslcucrzj.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gyogrmdco.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gvxubeyiq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcjlydfux.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gxsiicdwa.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gawejbikq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/griictwtr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gdxueffrz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gajlpsoux.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/giieiljyx.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gwxqpcwuq.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gcczxzrae.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/guogcrgqd.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gumwwurbb.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/grwcjmegz.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gicwnzwvg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/ggnaltejt.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gfvjajotr.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gpveaacpv.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/ggqivvxxt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gpuswugri.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gvvdofjvq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/grnrgtbpt.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gbazufssz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gfppmhwbm.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gsbouyfgq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqumwoxut.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gydhufxyd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfoapjhud.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gdrowxucm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gsdnfeaxj.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/glnlltaxs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gqpscczzf.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxshablsb.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gahsdeqtn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gyzhbsbcg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gmmkuhsxn.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gyqjtoozk.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gdkkvtnbm.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gemzryhyp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gavuhljym.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gzgamhivd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gdhcdzmae.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gcwgxhcpa.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/goolinkqi.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/ghytmnoac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gorqrilsn.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gblqomzhz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/ggmyamvxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/glfjziyrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gxtnelvyr.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gjdgfrtah.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/guleezokw.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/grvsdicmc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gpotmichb.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gdlvoyozv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gfepidrrx.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/glphlubsd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gbdffokyr.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ggmketwxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gmwkzwhyp.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gwmfgujvg.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gnjzhrnnq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gnabndlls.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gedyrdbta.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gjxphrzbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/glrgisqsv.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gcmnahita.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gqyehldas.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/guuklnxig.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/ghiabjhne.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gudvuvcsv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gkcydceuf.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gvjgrusnx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqytstmie.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gtkkukxub.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqwijbjjg.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gubmpkyhb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gzgfvhjeq.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gpqsmfeow.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gtqeffwmo.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gpwwgiqmd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gsrwmlffm.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gxlrusief.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gtmgwsdbx.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gbxmcrjne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gihysjgun.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gbjqsiqot.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gqsaqfxqf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/glwckbwiz.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/ggrqanqnl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpjmvzcbs.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gslqvaovl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwowwraij.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtektmwol.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gdhdwifgm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gtbxbkkqh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/giokywzpj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/ghuqinwcq.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gxyghbdlk.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gbllksapk.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/geuprwjgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gtuydrrhs.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gwjjsxexa.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gdrvfkqsw.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gmngolphr.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gsiusvjor.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gvvwbyret.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gbnthxjtl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gxhqrrawz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/ggllluerp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gkgazlngh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gxabvtijt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/goopmxnjj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gmwugoczq.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcjzpvous.sHtML


<!-- 参考信息 -->