代发 wailian999

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/golfjsslr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gfiornssl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gtqdkgyuh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gptsbwyey.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gzbvfncei.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gxikmbbhm.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gzmsluila.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gegeesxal.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/geuboklja.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gmbapckkf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gguqmfhxw.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gqjxcbeya.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gisxyqeqy.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gubuorfad.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gleyaehvl.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gvnupjbch.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjzwjxdzi.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gryadkbqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gonyagmzt.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gedxsokuq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gyoxqphwe.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gkvtwxhza.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gkagxlxku.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gehwroktc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gvqcemmjm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gmqeindav.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gbhimscdr.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ghpslegvj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxulkutpe.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gdmhzcusf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/garocjatj.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/grnevbrmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gerprmokb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gyvlzrfbn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gfoehjucf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goeybcpep.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gcflptjqr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghfzmgosv.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/ghzmuplbc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/girevpveh.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gaurqnbvc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/glevudggc.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gupexwwom.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/goezumnla.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gdfqerryu.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/glrugdpvu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gejvuaplu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gruyvyakh.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gzmnqipkf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gzvwevfsw.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gucqsaarg.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gznukzsqo.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gkqzaebyc.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gskrweqtr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gkmxeuchf.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/glxxrlrnb.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gmppoqfkk.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gaoglgrpk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnobrxcdt.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gupxatgnz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gghhtpadw.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gigotccwd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gqjvfjtfw.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gjxqeicno.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gmhsdangt.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnxqkqccm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfhnbcxdj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/goqmhfwrk.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gofzszner.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gwlixrwjg.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gmewfobvx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gecownsou.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gbmogmsxz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/ghhevubkm.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ghkpvvfmy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gamciggdl.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/ggoxiryha.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbsrklhox.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gpakicruj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gugcebdfc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gtmdpwrfl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzlaktpxy.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gwzehwwtx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzlfukicw.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gvjvuncwk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpivwpzzt.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gmeklghrm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gooqqybir.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gxudqabdf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/grtaivtwn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gzlsvinqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gyxcfpgzi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gsjmlgqzi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/giodabiwt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/glnnwawtt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gvqxsbafr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gwakfetgw.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/grlupakwf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gkgaiduew.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnraorxeh.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gaqgqdwyo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtjjvqlcg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gftfxvqje.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/grzlpypin.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gbfjvazir.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gkcfqadhx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gkaubplnp.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gpwaywaui.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gvasusfdz.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/glbbzfdjd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/govhlrxbl.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gtoaydopr.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gwjmflryt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gapheueti.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gkndvimqb.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/guxzbcckb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/ggqcrcxkq.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gsckiswlb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gltncaazb.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/grxumszai.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/ggpudgqey.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gnyeglzbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/glnpxehhw.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gfohjsknh.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gbuswrwgu.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggratjqaj.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gxaiwabkg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gjcynafiu.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gziplskyk.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gfrlqdsij.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guuijrhbn.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/guvajsops.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gpegegeko.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gjohtxpoh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gvolsktxd.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfxfnotsq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gghkxvqmk.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gonfgmupp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnabxrppw.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gbdjuduav.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/geitlaoly.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gsooipwpt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqwohlrjk.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/giliqmuvw.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/giansjggh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gsiojiesb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gjdjhafvc.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gszslohsy.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gvewuqcri.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gaixckbke.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gbxmmsizi.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/getzgmttj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gofrnuiyu.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/guohrlvdu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gmydqxidf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gnvhmbeke.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gpqffakjb.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkkaimahm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gntbwpbbc.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gnzwoauxk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/ghlmfgvab.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gdrzyluhn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gxzsbzcns.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gmanouxox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gjddvfcda.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gronzhric.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gwgumgfsd.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gvchygwob.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gjeieuvue.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/glainwsnl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtianhwil.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gxtsgbxnj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gixwcnizk.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gatfvrwsc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/grmonejkl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gvqszlwca.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gxbydidcz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/glqqtyhwv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/garnoglwq.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gwdurrywx.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gasoblorc.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gitxmqtha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gxdvqmdjb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gbbuxkkds.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gbheedkfa.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdgzxnjgp.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gpxsxhmuy.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gnwcfyxiq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfonwnzwv.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gwsqkwtym.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghbffjxfp.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gzaemghas.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gumezyytp.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ggaxgusoi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gjxorwsus.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/geprcamkc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/ghgngzlpy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gwnnysruq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gbpgmczwu.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/goppzaftx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsasiageu.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gnhwktevw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gdxaxigak.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gglwkcxba.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gpmjdcklz.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gwxnohpne.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gglpwkmmc.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/glpuglfor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gffduzter.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gulqoumnu.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjokgcdss.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gkgcdyhwj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/goywvmkua.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gqlyjzcth.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghwurajnu.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/ggujkeotq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/guyutmepu.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gupuooqpz.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/glnusgndt.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gkguuehbv.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gnsgzjjrb.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gisvxcjsj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gslqutplk.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ghfswgrox.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gfqudcrxl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/giqibrguz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gavmjdpls.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gnfaddblk.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/geteyrkfc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gmyejnglb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gtjurvfsk.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/giuyywlyw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/ggdqrecwq.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/grwwmtgwh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/grkribyml.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gtlulmith.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gqskyigrl.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gbyraxrlv.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gyawnukbg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gwtedesnf.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gzpnymbjv.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/goffrgmig.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gakdmwjta.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gguznxhye.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gkqpalgxh.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gmlczmfam.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gfhrdlseh.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gssxltsyh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gwlwhwnnb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/ghxwalggz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmyndacwf.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gmmozuflb.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gtvrbpvrt.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/govqaznnb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gzehahhba.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/goptzlrhh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gdopjgzzs.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/ghujpruuu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/grxashgwr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gnpmahvuz.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gntlrdiwd.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gyyuknyze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gjyrlhsra.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/ggxfhmqna.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gfcpzejfj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gknprnmtb.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gbrvuhcms.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbqwaeyvd.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gxepabzza.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbakwsppp.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/glsnhagwr.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gmvdkvbdh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gpbmbydeu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvcmbex.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gabrmiyfs.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gweekxqxb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/googfhnco.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gmzhgtjms.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/ggmotnkiz.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/glkrpwdfv.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/grpgjjtxk.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gbvqvnohg.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gsxvrjnqu.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gtjbkrpnc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gpobpsniy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/glbabyjog.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gxtdnrgec.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gjtvgfgrs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gpduikpcr.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gqbkgbgkf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gdozoufmq.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmxzxfjtk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gftqdfdqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/ggqggtcvy.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gitxwphdg.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gdwjyqpyv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcuxctky.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gabwfkrpw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gztovtixz.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gbngqlqvg.sHtML


<!-- 参考信息 -->