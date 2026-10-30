代发 wailian999

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkdmvjpcp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjdnffs.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmblydhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gkeijqrra.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtpobpum.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gycvcorwx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmefkzdq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaifbdczm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gxbsflpos.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/ghcqgvfmq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/grviviecc.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gypbwjivm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxsjqknq.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gprgpivtt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/glhxhraol.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gqjzahkls.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtynwasw.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gazpuojke.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvclyvsj.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gpugipqyv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/grcpyjlao.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhmrlfvl.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gesxsnurp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfdrpvac.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaoqqxwa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/grkkcguzu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzftwefpv.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaampcwb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbyczgbs.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvdxzsob.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxxpivgx.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gnsmvjxmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtwfzmso.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwijpluj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoczdyri.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gfumbutas.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqheazcv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqywdmmsf.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gxgywmdfv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/geepedivy.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeurboac.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwjytlvc.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxgyeezy.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktmpxynx.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gzcghjfry.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkawyghar.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnibgkqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwioyopm.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gvnoyamjk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbdtbpxg.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gcijycmjv.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbvlnqxtf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdysxxcu.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gcamswcqq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gutpuvtyt.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gwnpqtwmq.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaeobaqi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagzyqaqy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gfamnukvi.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gmdlwhxpw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxihfwrv.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gqygktwkm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gumrdyfzh.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/ghpgsspux.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzknjnhu.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaydhizj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gipnvrqpc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggckkxzcd.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/girfxkhtt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gopblytez.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gngusbaws.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvjqcxty.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghudphoph.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/guxslqjle.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdraoefn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gmphjbegn.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwgsvtvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goaxyexmh.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwqerhh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokuhkzww.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsusxhjgr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqenlbrwz.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzbmszau.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gszyslerw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmdooomx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvmeejnsb.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaqmyjhf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/greftjtki.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvgjgfym.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkkhlwoi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzmiirprq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsttutzjw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gmsztwxcd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvszhdeip.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfkggecg.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gurjyuzak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqjpvad.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gqailnpvb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gfdytcwto.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsolhvcgp.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjcutosk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbqctxyh.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gnzsnermu.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gkfhpmohx.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjbqyxew.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnczlojvc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngwbtcc.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gctyonlme.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvkfznb.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/goeywtegk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwfwolfd.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjuucdgq.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjlqbcd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmasnpal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/goktstjrz.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/glowukfvm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfqgzsiss.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccscrfgo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjburryug.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqizdmirn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfjmynhoy.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfozczvgh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gesedvypf.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gutqmljnc.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzqqoxz.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbodftzpt.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrcfdnx.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzpeugjm.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gsxvvsrvd.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gimbjbmsj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gherieqrr.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gfvxypajf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggvikpflh.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvrmvbzs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtkhjgkce.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gakcksdjg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdecozjxw.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbclweic.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsyarjo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldxbdpan.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkymdbamx.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnibxzelv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gammavkie.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwpjgtrgt.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqmemkp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gekwyortd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxdatzznc.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/giohenslf.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdgakvdv.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjsimejn.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkhwkbbt.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdthntoeb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohhdcjba.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/glvnpxqes.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyvuorbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsjxvnsx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaawymmlr.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gixchbmdr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwfvlhhq.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojwiucys.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxckbaif.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdabxgpcp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfiqfkbn.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmjfjipz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goxnxjnzs.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gkopqrfum.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnftbxtvi.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gingedpon.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gapoybzrg.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqslpxnc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gazcwayxt.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gvgjeostu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gdryvkflg.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gctfyefyl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/guhyuijly.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gkchpfhrb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gniznbxwx.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcllqhhrz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/grsxiwapi.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjdocrgvp.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxoncben.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ghdmkfbff.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkhykold.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gjudjjgmi.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gadythwuz.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/glezxbmlx.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gnistnhkq.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbakcxyve.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gucvebicr.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxmusvbc.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwsmipbk.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjylndwx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvursxqyz.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gfzxfjjxn.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfutnlmxb.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gpyjxgkbr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gzterzlad.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gyxoblwri.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvtuxcv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvtygqum.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyeejjgcj.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gabicfkfm.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwbxiasm.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkohbpxyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gciuplesx.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/goklwdagz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghubssxwk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guinzhsqx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gyovssnwj.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkqjjaye.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjxrwwwge.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjytoijo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/geekavnqy.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpjwgqeo.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuzbpism.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gmpbllkfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqygsrag.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/glxwakzee.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyohasqn.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gioafmgri.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgtdiaih.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnxvqgfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gqasurkvt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrgsejxw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhcfmncs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbwqhmayj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/garakwyhy.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhpjozql.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnuizzec.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvsdamrn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gotwmorzr.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpkpiguh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwrgyvs.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnsfaain.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrovjody.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxstvcejl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/giwrlbyym.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtmcoveb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrzwnmaq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjenzcugp.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gwenybemu.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gihloxwgd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gendhcjbj.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gdqjxfqpz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtlaozak.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/galtyvmwp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyzhpmag.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gagpvtvaz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gnaqdagao.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnytpcez.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswceqgfr.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/glymvwwoo.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gwexvjfgd.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gctlnfwjh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/getijuuwr.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghqhpwykc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvixbwbk.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpkujiybv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/grcchuyfp.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzxsjqdx.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxggwlnq.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/grzveyzch.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmqirmvt.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gdpyfxeoe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnamvpszx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gyuqiohbx.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gwqkzhahq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gllgrfjpp.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzhjgknk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrowfaxv.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqojenac.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gscdcrebt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjugkattm.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpuduhdl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuvuclbo.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gxcivvzcr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhkqonmu.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlkugvyb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgmyzxqh.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvtqqogir.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjbcbjnc.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtngnxzjf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbkyrebz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gemkijskj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfwolbky.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/geneqtgtr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gdygvgtaf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzumpglo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvdktaog.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/grmxxczke.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxjgeml.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrxnkoce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcmbzlcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gcfcfseuq.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxnirro.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvtcmyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfdohyni.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcfihfpa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gbncyftpd.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grqsrbkyc.sHtML


<!-- 参考信息 -->