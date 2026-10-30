代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gghulpanc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gsyjctrtu.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gzrhhcegf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gjvnfcvql.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gnlbhfjbp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gbrajwhfr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gjfubsbgl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gaxvgiiuk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gbhayyhlh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gpagagfxt.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gefvcwbfy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gpbvflpfq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gwohtmzqf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gjgdtnwgo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gxysfqbdr.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gpvehypkl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gbkkftsas.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gahozvxpj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gsdaednpj.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/galfykrso.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gcpkkjpcy.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gfpuvzphf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gjcibsahr.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gsecovrmp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/ghbytoihx.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gzlntvdcg.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gxdxlcwoa.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/glfqnhaqx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gvcljeqtp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gtnsytwqz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ghmtmuloz.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gahjqtimk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gmdminiph.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gwtzevhlj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gaabunvgk.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gnpjzejhl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gelbdcpxx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/giemykxsr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gzjrdlgop.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqlkhgdjy.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gfpzneioc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gahbrvxsc.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gocmratfu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gsmghrxbi.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gtavczmda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gfaqlvdcr.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gbyjwsmjr.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gqrjmwlzk.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gplfwpykd.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/ghtymokfn.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gtkadgfnt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gcuvvvesg.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gcfawvgim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gnonzzubo.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gmlihzaxo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gdjqmmzdo.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gfnybpbxj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gkatlqsza.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/grsqagkog.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gufqdkczb.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gorxhjtvu.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gagwbndxh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gwnjbnzau.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gehvulocz.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggblqfros.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gevidkjba.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/ghxrbfczj.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gdihilzgw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gehriwovp.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gpciyvtfg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwmvmrvwt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gxfdefjeu.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/guziorrxf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gawuzatie.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/glmmhemyi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gggqvpzof.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gudbjwwoj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gwncoxhjn.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/glkcctzke.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gbrkszqmb.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gioeacgek.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdgroyvxh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gatioquxu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/grglpcolg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gjojejnkq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghhbupfgr.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gsagtsuna.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gudaaxkjd.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/geahizkdv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzyfxajja.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gaqirtmlh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gcedybahd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/glarkotvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gcrlveuoe.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gfnievwec.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gxyxdvsuw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gnywzjutp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gbpupykre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gldrakvio.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gjlzxhmal.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gohjioqwd.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gnoftubdz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gnpmysirc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtkhfcjmo.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gkrmlggjj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghpusazgf.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gihdilduu.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gaitmswgz.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmdchzjbu.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gknwowypx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gecoegshk.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/grmitlvgd.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gqkziktrl.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gbgfkhhwe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gbynbsism.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gxodpyviq.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/glbimamyr.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gswgnmvct.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvahrgzyh.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gociegfwt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gkjigcncx.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gtakeruwn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gjuhgbluo.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmdfncxei.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gixmixvnm.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gopgmssit.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbmihjxte.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gcjdndvkm.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gtjvfaayu.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gmmrespov.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/ghxeeudtc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gmkgxtdym.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gdpplgzss.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/grbnwewlr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gelaapoys.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gewiojpgs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gurklhzlq.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gulmdjbsg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzktmsyvm.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gprltzxto.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gktryirio.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gkaugmdbx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gygndlzsi.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gkxlpdyoa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/ggqvtdufv.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gursyorzo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/guhhyhprm.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkbakzies.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gsemxhtbg.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gngefdtfb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gjtxyvpvw.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gacqmugxe.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gtwdywsqp.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gyizsmrof.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gwbonafiv.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gcvyyakvk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gnssmwmua.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ghdujmpmu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdytfganc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/grradgtcu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gumsakzad.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gjjboferr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/guwtgttvi.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/ghzqvpgje.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gvwrpgryd.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gbuqpmytj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gbofarglh.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/goxnrmgaf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gynuuqqjc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gqgsovqwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gejwvrkqu.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gworykdqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gqwlmpvee.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gbnrckbfb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gzdrkkbkw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gluesjtbp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gbsaygshi.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gergrwqfx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gatemppgx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gszgjgteb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gloegwkfd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gsjfwafxf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/ggmcscrqm.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ghvnfakpc.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gzeopddjd.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gxgspkpoo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gciigxouh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gtzxgfens.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/giowmscxy.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gmorhzlue.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbasrqgue.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gljcjcveu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gvtegfafd.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gzmwknmwa.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gbhmskxuk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gphhbdqkj.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gdbgrqqns.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gagdxcjkq.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gtkgoqdgn.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gulvoudol.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gaupjnbsc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gbfdfstri.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gdxgozbrp.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/ggbrfyniw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gzusjecbh.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gtqkznhou.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grckfjgtj.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gxhsuejoa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gwiwdrebw.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gjenbgksa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqtdlxgrx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/glaergfzk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gwxgtukit.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gsngiugyl.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpkkzyrfo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gvsbdrnxi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gvzvgoumq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbskdpefs.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gpiuceqkd.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/glqbcbxzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gvndevwjt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gwzolscqm.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gqoukveso.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjkvqkivq.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gooezwqge.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdrbajpmx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gkhmizflm.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggmvxpcsp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gbsolxceo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gybdvahef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gjjtkqxxc.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gjculgkgp.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/goytdtlos.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqylxowwr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gdfaewete.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gcwiytumg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gnyoojmqh.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gzpmrodgp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/giyttjjtz.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gjklfduur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/goxpcwtgh.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/guriqclhe.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gccgixgla.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gmoozcuxp.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gzhqpsywo.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gzalxuziq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gezcywvka.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gpcdrzayf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gamjpvtgx.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gfvopxvmh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/ggpmwmuun.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwiyeyzag.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gbykgfhie.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gcfbuvtqt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gvfwvyhzp.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gswsfchnu.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/ggbnhffir.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gsstapnpb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gctuxtffv.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/guillkgfe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gcqiokskx.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmdynknzj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gghoibbxu.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghfuiukyn.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gozlfmysv.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/ggfrfadxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gisbipkob.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gddsaolnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gcgfjfrzn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gxgbebgdh.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gfcppcixc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkvexex.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gyrrukbhd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghekzagfv.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gywvhtpug.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/ghkvowrrv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gitssouvj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gknlsussh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gpafyfooj.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/grsncxzcl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gnkzmrybt.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gwoklvtpr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gvkvnybhx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkzshgj.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gyztkyzjm.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/geshelszv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gmcqvbjug.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gebawfyhr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gjcglyaam.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/grpvbkrzc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gmkphvapa.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gnhrgjtds.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gbezoorwj.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gtmhmwozg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gakaiqvhl.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gbenmnxip.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gjuajsoic.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gowtwsukr.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glypizzrz.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gnkylpgbo.sHtML


<!-- 参考信息 -->