代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gpmbfxnny.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gbikiepph.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtjerivpm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnqddzeu.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzgbxyh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijhpvfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqsutgeh.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gqigdpefe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gecpailnt.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gievskurb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gczhaxotv.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gurybrcot.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeortmui.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxiyfod.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gungnxfmy.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyomnhob.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gntgqelmj.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gqbsrcpcr.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgdkchoh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbujwchqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gtfdotgpv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvshkgs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/giagcxily.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gwadvhzcd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcizsiuzy.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfrranzw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnnzumglt.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gterhohwm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gyokxfaii.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/geqgldrvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gthaolags.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzfnusgp.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gxtsxwadt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjkwmwuib.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gblivnteb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gazpwjkyw.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdavcjnwr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/ggnqslgwt.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gwdqmkpzs.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyszaerzu.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdilhnsb.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gfiynpnlz.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxboscca.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeladixj.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gtexzuazd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gonxhqrlo.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gurfxlxin.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfilryae.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutoeapbe.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gstawcpzi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gnqrqkwdx.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdootthi.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmawtpsym.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibwcrymy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gvygxlbxs.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspcoidbt.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxccszpex.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavsmvwly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxqrtncm.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwdyhghi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gxkdyjxem.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuumvnlo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjcpzohca.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gagsudbjq.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gklooqlkl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcjtble.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/guhpjjiak.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gbubexybx.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gugdtorax.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gftbmolug.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsffenzl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/ghikzovcd.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlexqfuj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gisvyirgn.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgtcbkac.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goiibfcju.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giehmnjpg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxdzlum.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvbzzyrje.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbjgiqwf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabkrclag.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqblwtwct.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwthfuyyw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmbjjsbv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/goacjirkm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgzzbcej.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvjrwpfju.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gwxgcawrl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gjwzinflw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxemlhiy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghkuqvkbh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqirblve.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/glukttahl.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gimtrshgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gvlfpecig.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giylpavxk.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gulxufaml.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqgwazway.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpizplmwa.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gwbmtegsf.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfmgpoxd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gwhxsatnr.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/glvhyzmcu.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkgqsknhg.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbctieqw.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwkubnml.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcartnmon.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqtakqwu.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbbkafbem.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gtjwgsnas.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxpvwgmh.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/grlcojgyo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwkniyhc.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdukgmgmf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqituftdd.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gziueoexc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqjrnhxov.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gasfjtqdz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gtgetgyrg.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdvwwtr.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gomrvlagv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunodhbos.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyspacuwr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdhmimzp.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gbizlumoc.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geosttwkd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grdsylgpy.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurmppmct.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsdyveeh.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsxnllpq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqzmthogr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqamhftco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfncegwoj.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/guyltqipz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gykhzootv.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzmyrlzf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwrscrnig.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiauqcon.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmsnvvfr.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcyrhkgva.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekfjbgkw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlxrewup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gojefamlg.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gavlibcni.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grnbvhzts.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjwiduwt.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcbqdbqnu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfnlruobw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzozfhbb.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxglgvifx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggyiuqadc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gkzatwypw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzmgvbqc.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlojfeaw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/giyddmwbj.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gktnvdegl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfjnlqib.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggohtriqw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gmyboebau.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvfgvbwf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevotain.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ggcvmhvxh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeyrrwfm.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggppngviv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsxodpgc.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gqhtazilv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccoivrgn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqrtfuhd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gbzskrvds.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqoiroy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gsmkwjfhl.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ggdzqhiee.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gsbuntewo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmvfqeil.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvoqyzunk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsowvcyh.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glopfmhid.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gfowhiqat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfzpcbxi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvntrjlqc.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpadczmji.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbfyevhb.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdgmjtyn.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzftblmc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbeyetdtm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytrvplez.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqsjmssn.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiiijvtl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimynqra.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexsppyze.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gopcwazgd.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gpcqzjbfe.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gkacyttws.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gotjrafmw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gynazkbps.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsrfhomzi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gojqtnpht.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gbgnmjkrn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjpdldmg.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwcmwfvf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjefybovb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwyxuawbh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbzdaupo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbgjlgvp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gqchrmhdx.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/goksxwbsy.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzptfmglf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gjpxtxrgh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpnkbatvw.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gafqvepxv.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaiqrkch.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcmwslke.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gisydtzbe.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrpexhra.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gwbbfvvet.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/geeykdega.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwaugzt.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gopfgzgld.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdjrzdmy.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwcsjlbx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghsiethac.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gttjjstud.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlbjzcue.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdvviovqv.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbtrllja.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpiwynarf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gyjzikyki.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghclzgibp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqoxorabg.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gazollmmn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwgetyrf.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/geqkbqneu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdexwjdkr.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjtequjk.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaeqvseh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gxdfxibjv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenikolp.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/girwbbmcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvwqjqqqe.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/ghzxrumaq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkccwxwip.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbntfwujm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gpjsdzehz.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqwovkuoz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxexeppu.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gnelzlylo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxvnlgjsc.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkgustkzf.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gxgujcjlg.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljtfpwww.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxkboxbg.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdxezojm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gttbmnytc.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnbgrzn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfrbgvsj.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwsnnkqd.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsqzstfk.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gmpmvbcsb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/grnjpgnux.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gqesgmrgi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjhpbjmqr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ghzuigrci.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gmseisujr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxydskpi.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/glagosczb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrnyzmpa.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphjwsmib.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gusrhqxcc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdkzimktu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqkwzfbuk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbbhangkx.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/ggtlixqmr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/glywyzxha.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gmcpmbadd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/guozvhvah.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvbfpmlb.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbrwmhpxb.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gghizgcpn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gfitqzhja.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glwufcnck.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjahdyox.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzuqzmmv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gmclxblvr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvndlajos.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gopchjtiz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrdwusom.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gblwysxos.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grtaymaaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjravurgl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gznkygnby.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glfanpoya.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxofzozhy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gulqgkwju.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrrahxdm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/guqgzfarm.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbitrwbsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdxziuv.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grudmisdp.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/goljzrehj.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdvxwfm.sHtML


<!-- 参考信息 -->