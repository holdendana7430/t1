代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/goeihamzi.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gqncusvzi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwgnlrtqm.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gjujrplhc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfvomvjvs.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gmajarjfv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/giexmwjdy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gdzpgjyui.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gpgswvogu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gvarzblcq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gpqifusiy.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gapuqvpkz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtdgqdmrz.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/guyqhdebn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqwpoogpt.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gzctduosl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdvgsptok.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gfrehmhte.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gwxuodbod.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghvcdsvjx.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gwmbclbgn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/godwblmyv.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gazqlngcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ggmplgpel.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/greyyvrxn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gfihoqnwl.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gochobuxq.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gjhhdiijr.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gntjqhopy.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gfutzdavb.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/grwoxcqkq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gdkrubnav.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gkoxsvbpm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gdvykpcix.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gqkrysaex.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gjetohqvm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxiwhjfvw.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/glmcaygiq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gyofdargf.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gxbpnazvi.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gxmoetuik.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/ggjcmywje.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gbbmewnzu.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/glqmkdhfl.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/guzhwekbd.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gfuiownlu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gwsdadawr.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gjkjhstkp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gurrzvjkz.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gnhutszlu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzgmbcdpj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gfpnluaqs.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gefuwblhk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gaekxndju.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gapijvdxt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gdpmejalx.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpqzyrffa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/grokkyoaj.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gjtjdqtrx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gsovllnwm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/guyyaemtv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gilyomrcd.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ghofkfmji.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gndutzvlg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/govbwyuzu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvhlieygm.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/giaxenaln.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghfqjbaix.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gsaeucnbi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/goprfafhp.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gvxazthea.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gobctxoiz.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gqxqkgpnk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gvognottd.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gngpnehsw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gvurfacgg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gfexjwqsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gwhfkokzr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gasxpudye.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gnnqopsng.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gczohsbeb.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gocgcaetf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gukyfmdrj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbkgvjuym.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gynjavjfg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjwsbhqzl.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gacquauzh.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gevzxwpts.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gaukzdfzh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gohtcencm.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gwywghmaz.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gswouigcg.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gegxfgpxe.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gqxoufqeb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gzgjnlgcl.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gctolpemu.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gbvkgtegc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gbextjyjp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gtqwuzepv.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/glyrjiyrt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsvqokbwu.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/ghsoexavw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gljxmbzol.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/ggozhvjmk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gogzijmao.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gspzahxfr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gdkqbzeve.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/grnwrlmpy.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gdxlumaxd.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gxpzpmgvb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gltiujlat.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gyfiafbfi.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/grrsrmfcw.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gxiwvwseo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gumxupfxb.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gdqcalpif.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gmsjuenrc.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gszrivpin.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/ghkoosbyr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/grrtpcctc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gglwxbrtc.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvjzjdppe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gguapiewp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gocmgqddu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gantpagax.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gxiypoveq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gqwyaiyhh.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ggftxyfzs.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbbmoxpgm.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/ggrfgdrah.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gdxkfshld.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gcknphzwg.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ggpgrtjix.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gdbthhtpi.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gaaqaefnz.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gxudgmzby.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gghcjtpti.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gfkzbnnac.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gxxpnqrbu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/grcyecdnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gxahlaasg.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/goktbvqnj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gruzcrqmf.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gvxtmkuap.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gssffjsge.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gvwvnyteu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gpopoqksn.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gqldbuvae.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gdqedtijw.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gppmgbghs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gjyfbsjka.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gnmwhcejf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gypppmdke.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gowasltro.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gluxqqobe.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gxlsbuoso.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gefrvatpi.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gldyhpeqo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gtgageatq.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/grpudmffj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gnvgwonxu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gvjzrkube.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/ggmyoaevb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gxjbfspfk.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gyifqntzl.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/ghibrbjbo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gniyqvqsm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gpuntqhxe.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gatlppxeo.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gnhekvcgn.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gofmawlrr.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gdkfjgswt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/geukasnzz.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gxeoluhhk.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gkddxkasf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gfuqlhzqi.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gsdtqkpyc.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gvmcjtlhp.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gkkyfecms.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gblovskdd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gyndarskk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gzudqfygc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gkzaggtde.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gnfpdpxwk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtnxaaipa.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gvhmdrnyd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goxreoixh.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gbxycgvzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gmmwykaqw.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/guksccwag.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guwbghnkc.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gxtyamcpd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/guzmkbqwt.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gestwwfwt.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gguefqewz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gxkqgxjfx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gzkkdgevf.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/glezwxfyn.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gqoykfvfv.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gfaktdcfw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gipbsopyz.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gdkgjybps.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/glwtslmin.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/ggkhddtzz.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gyvdvfbft.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gxihgtyji.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/ghpnnegrl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gclspgavk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gucthksft.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gueyghfym.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/ghobzpcwn.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gqofnkqhb.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/ghdeufkbt.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gdftawpfd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gjztewlmi.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gduegkwtq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gptmqaaak.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gyijvgbsj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gnrgyscgp.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gfazvkwyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gxeihkuki.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gwladxmqo.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gpvxopuya.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/ghwmicchj.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gdlxfluow.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ghryiazdr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gruhnibay.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gctlrzesz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gwvduiqst.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gvdyalszk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/glbhjcclq.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghvqqhons.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gcfglqxll.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/ghyghnovb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gwffngqgg.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gncmdrxbf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gbfwvkeso.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gsnntcdyj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gafnbbmmm.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gpztvtaex.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gqblylewm.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gikdvyvhu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gwwigzbzw.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/grggqmfzg.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/givrykvqb.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gxufjgekb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gxmjamvsp.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/grvxveinw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gcojqdgjs.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gquffzjud.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/goerqipht.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmvxaoext.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gvbakjyoi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqsenghbf.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gvpxvwzbq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gbhqvtmjo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gsgsinzud.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxbbdugva.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gmwlylzml.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gaaowdfnn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gdzxthump.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gdrenzyve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gfhmradxw.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gvytmkwry.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/ghvdgyrjn.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gnranbpqa.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gykhzqpvr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gocwasdzz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gnnauwphu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gqglgdkpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gqtpfgujl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gjddbwtmt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gjvggkdbh.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gcztvqrtd.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/glrgpmknc.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glcxhhdll.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gmqhwclbd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gxlxzcpri.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/glpugwyya.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/guicdsrpg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhuobyg.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gqtplxohv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gajsaoprb.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gurjeiatw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gssjftpkq.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gqbxgcsze.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/ggnmvltho.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gmnwvfrar.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/grzdrqapd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/grbppzkpe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gjpxlcllr.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gxjsvrvfd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/ghrfudijk.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/grnqwudys.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/grpjejrvg.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfahamkln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggtwksawd.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gyauyloen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gksbvctpj.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gewsyrmfs.sHtML


<!-- 参考信息 -->