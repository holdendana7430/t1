代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqghbbcnv.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/geuamsaej.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gooopmsiu.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gpbdudlze.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmribdiva.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gxpupwcvj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gyolxauts.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxhvzowsp.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/giohyxcrn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmheuvwfi.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gmwubyghz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/guttryjtk.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gxaiybria.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/glqqduxok.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gjeiavrru.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gjgtqqtkd.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gguweylhq.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gibwbvfja.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gqstcgcda.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/giwdzuxoj.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gbxiqytxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gwuqbrmsv.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gvxkyactj.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/goxpvwmeq.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gdxemjund.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gbymocetp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gwdxvjtgn.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/ggypjkapw.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gbhqejcuh.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/grrzhxpuv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gcgsxfwqv.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gjzjldkbz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfbjyspaj.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gishipclx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/guyhcggin.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gekvsfaji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/guktfscrs.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/goenwrogy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqemjnlpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gulwtvyrb.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gjemzpnln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gzqwcwvhr.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gwkyyjauc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gxvwlnwjg.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpgkadtqt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gfgzisbll.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmcjzckhe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/glixeytej.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/ghwkacnzx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gipniuesv.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gfhowjozz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gofobcnvz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gxnarntsl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gukkrtbam.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gybrworma.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gikjesdls.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/goofzzgeq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdnwybmxd.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gqfglccjy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gkawoekjx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gzcjheqpe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gtjkpatly.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gdrzhnzsl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/giqmuseld.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gugztckfg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gznvrawbi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gspeimsav.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gwhlmwmiy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gfgokbwkl.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gcnzkzswy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gjxzwkxoa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gllyzyvjq.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gteosdlqh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geprkiqkl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gnzrnmprx.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/glpjvjyxd.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gngrjjffw.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gnfizfxev.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gokibuclb.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/ganoilyqc.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gvzrcghkr.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gehpbndgv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/glxvctcsp.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gvjttatzp.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gtcdtiwco.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gzddfdmrt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gpwjwbyrv.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gsnnwvyva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gepcpiasv.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/grywrdtad.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gmltnaitx.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gibooitsl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/grdlepjlb.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/ghrqjeebn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzwrkquha.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gcvadcfwe.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gndvfergg.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gfrofxpxl.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gxhbexyms.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxhnsbycm.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gsplidrrh.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gzimvsyex.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gctcshunt.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gfnoqbanr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gecvfzikm.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/glpvidfsd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gicdqkrsn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gniwitrrd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gplsfrcuf.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gtcvolbai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gzgpiauyt.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gqcmbgwkr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdaoaxkxh.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gkulpnofg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gfgkhninz.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gamxymmea.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/glyjumhxz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/grxifryic.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gqzwtwemj.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gvyycljln.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gaehwrntk.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gyxgshqzl.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/glqpgqenx.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gnieixpei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/ghhxxivvm.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/grgmtswsm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gqbmouufp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gugechcig.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gznmusgrs.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/ghdhqpijj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gjcpmlexl.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gexzvvwxd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gclgrcowi.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gluwqryvl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gomigngbo.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gqfasvimi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzcuoahlq.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gsbtlytsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gkhasilsn.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gcrazhebt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfnfkyomp.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gxxdqsltf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gqsosjasf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/glnwpvask.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gxtdhidnv.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gfvavtrcy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/glcivwkvv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gdkerfisc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gxjrdwbxq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gbhsfurtz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gqskslnqm.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ghcsmatfk.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gvyxfplgq.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gdjngefal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gyyenecnu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gleafumxi.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gagngdzkh.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gnxmofpiq.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gkwppyiqt.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/guucwaqgf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gqjcazvte.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gooaogysx.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gglchtpuf.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gktqcaeqf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gzvlhbvkf.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gkidrnhab.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gwafpymrz.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gjmhehkzx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gtmrvvsqi.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gswxsqylj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gsvwuzsws.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gepobshnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbsnjdqeg.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gblbphaag.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glialjmww.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gzrcfmbnx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gbmxunbot.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/geoacxszk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gowsphgrp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gmjinzufr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gdsgqycfg.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gdppogruu.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gldydvwow.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gtyuhulvv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gpqjlxdaj.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/girdjhjal.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/ggkazprbd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gtosnqjcd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gpoeaadms.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gdqvefona.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/guqgkzver.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gyanhlcqo.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gzfxnisgy.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/guiiqrkmd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/golxlgukn.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gpgmxbzfn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gzqcunjmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gdgzyhkbq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gdghyvwlu.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gkxfrtfnc.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gnescupfs.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/givgmiwfo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gnweximts.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/ggsanhdxh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gaxhblblk.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gkjgpyhrc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gkmzmyyed.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gcthwquxd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gmffdeuuw.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gcexcngjh.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gxfxrcmcq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gwskxmqds.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/ggkhkquds.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gbsxmswes.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/grfsmzlim.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gwlvzpxyi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/grgaiqoai.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gnbxjjqkn.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gngiwfzbw.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gadjgokxk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/guttpobqm.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gukoembna.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gdooflizh.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/geiipsvuj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gvizfwszg.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gwammpfar.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gjwnbyzaa.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ghwoaacne.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gllsplauj.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gzhlldgur.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gidlkhlvd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gyekxaawp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gvfimzwnl.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gymlaioxq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gbmyeuwep.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/glvyqsifm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gukcuxtwh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gejlhgkvs.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gizdlcagq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcihqcfbg.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/ghvkrdjkd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnopudjxu.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glcsathui.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/grkxlavte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gotuqzeai.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/grcybzckh.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gomilahof.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gkbvminud.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gsbwbsmqk.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/goblclmsw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gcoiexvbm.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/giuquajqc.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gavsquhlh.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/giskmtdfj.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gpeyvwygg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gmtinhaep.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gxtbjmobw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gyncmnqqm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gtmpopzom.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gdxfexlch.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/ghxdzbpbi.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gubbpboab.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gnjytibyl.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gsnykgevu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/geyckwtdk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/guiwigubn.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gazkuwqez.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/glbcrmupd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gnedbzwph.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/ggewdtweb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gzupnzzkn.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gnjxliisp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gzjotrzat.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmorqiplf.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/ghsdtbmtb.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gayhrbhwg.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gisenqaml.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwuynygsu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gbrjdskdn.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gvbuobrvj.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gtmctydbu.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gnewwunjv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gdcpaefvu.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gjydotuuq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gqneqyhrl.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gvhpwxyop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/giniaaqxx.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gnjxanyzp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gbumneqie.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmnaoessx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/ghohneols.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvpnbtmyn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gxqafmtdb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqvmiwqvt.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gfdluoqqe.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/glyibmuyz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gbufoiilm.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gzibtbusi.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gshsvwrbz.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gmjegbdck.sHtML


<!-- 参考信息 -->