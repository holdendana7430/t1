代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/ggicedrdn.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gbplqcqbf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gukrafsqm.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gcxxbgsor.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/glslkiscu.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gfnppnvtj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gnnrfextf.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gkyrhhglk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ghyllovah.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkzfiksug.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gpipncywg.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/ggfiuoxfz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvvebmrfk.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gvsxbaejo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gmzyiabau.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gedcvnggz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyesiwqsu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gycnfjucq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gzsygclvn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnsswyqqw.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gjrkpjlvz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcdnylbap.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gwuiozglx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gsponegmf.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/ghzxkbnys.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gypartpdg.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gqzhqsxqy.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gwwisoqlb.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gmibtozwi.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gyhkyiqqw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gnkkwsnjz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gfiqavdjb.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gxmetfpfs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gbzqextwh.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gtxdyvrqx.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/glxnybbsy.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/guugfiztz.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/grbyaoyov.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gbroewxeh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gyeofnors.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gsmnqlxgm.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gnwkzyvox.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gwgxynuxp.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gbhedrkwd.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtdqxxliv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gxkdsxikm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gerlmuhsw.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gxiqcpiiy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gmruzseak.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/giqbsynqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkkofwlyu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gvxsdejez.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gnnqzvier.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gimozgpxj.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gjlvswhdz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gleppbrfl.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gcjhocqgi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gedesulwa.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gntsxprqg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gtdlmnobk.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gyrofuwjc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnaymhore.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/goutqitbg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmpofgtna.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gzldptect.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvvwntuks.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gziqgzlwz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/goysbedpl.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gaooyhnzi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzpoijhrv.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gfkyedfpe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbqhnebv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gymdhvvgi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gszyzbynv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/geuhpeobm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ghbisbjrn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grihsduxc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gscghfeeu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghhtvgwio.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtqrnjtyv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gcmzqxrbs.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gunoqfndl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gjhjbwfvz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaamdbxgp.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gsvdtmknp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmeontjwg.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gkkvcdugo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gztgpnmrj.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gtplpgnzi.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/glgktvdqc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gjqmsogqj.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/geyrdzamc.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gnecduvfr.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gjxghwinf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gjbjufvyw.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gwqvnkibi.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gpejznyrn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gzlwgcerz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gxgzpodbp.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gqicrqiuz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gjsnypjto.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gymujhdvj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxqfsifwa.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gffusfosd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gbnjhjwsj.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gtugzzfgl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/goanxkvnc.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gvrvlovhd.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/glyfdncjx.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gogmnwibn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gladstwcp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gplpktabj.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gkjobvcyx.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gqboczfjf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gnrxznizo.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/grmymhtsv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/geoczumsy.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/grnhoumzo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/goxmsfkqo.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbfnlzliq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gacmjeekq.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/ghgdfxnbc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gmdrdzyst.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gjueblurp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gksidiutm.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/glhclvhmp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gmzcqgxnw.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gsomkmdju.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gwrmsgnww.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gbmymocjk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gjwfgwhwz.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gksoagguw.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gsbcyoitb.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/grgfwhxcv.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/goiugqnli.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gudflynrb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gndplhxto.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gorpawoyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gaflcytee.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gtouwwzhs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gbnootukc.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gkjwigory.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/grpbqsloz.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gsruvqzez.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gucxrpxtn.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gqdowptmo.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grfvkuheb.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/ghequunva.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/ghzhxgmir.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gebrxecjw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/ggymgzlmm.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqitsinao.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gzngxbmnx.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gnhwiyhrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gbyzceoms.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gjjsqixuq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gjoksyppn.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gauborwya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gurriower.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gtaxttoxx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gcjrzjrvg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gtwcbkarm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gggviswtw.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gqinzwylr.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gnwgujuyo.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/ggeomunsj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/glwkqduns.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gwqudvrwy.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gmkkaljpu.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gxvgslgyf.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gtyerrjqg.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gzhnrlwff.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gtcljarcf.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnfarbe.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gzggmfhny.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gcdxaciqb.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/goftyrlqm.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gnmredzrs.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gbwuhxsgs.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/ggwgwlfdp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ggluihxun.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/grftrdzxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gkjpwparv.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gzmzbvfpn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gffefbcec.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gjzfdjboc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzsvhyfzq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/giqfwcexh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gloivccrp.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gysdouqum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gxsbqmuzy.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/godyygixf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/genbjxqwr.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gzcfjueee.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gajuzodws.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gildtkrif.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gqecdjtja.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gwoojhssh.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/glrhlnsvf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gkcldilkv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gvunxpgit.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gsbvnlvtq.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gipydszwn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gpfqwrwqf.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gonraxaxc.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gczacrcyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gxbqjvfnm.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gampifqjp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gslxznqtn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gpvvnyrxj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gfwctyatc.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/ghzmmzfrx.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gkzcqeope.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gwfynocpz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gwwqhgkrz.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gsddjlhkp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/ggrozfrhj.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gxtbwtnrb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gwfmftcyk.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gwgyfofwd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gnpsirmde.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gtlgllolj.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gnamxyngc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gaulavsqc.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/ghqfjbowc.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gghojvtte.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/grpsziolo.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gtbkbabih.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/govjyipwm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gmzaqcngp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gextbecpy.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvaaeicne.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gsglhubhy.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gkipftmax.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gyuzythnm.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gmoieywzs.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gboxgehfj.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/ginajbhwb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/goyyintzv.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/goauwxmkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gdlutbhna.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gkgvnxgzf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gkdhmfjwj.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gywpbgsmt.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gpmvtwgbj.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gkmidckwv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gpjevsbdb.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gllfqvwce.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gvvpfdfmk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gsjxqzmqn.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gchynybct.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnqrmuovw.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/ggqlglotn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkqquvvbx.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghzwszziy.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gogigmzmw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gbquylnbl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/glivddkwo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gwqjzeudc.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gdpxafgam.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gppfzfcpy.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gjfgzkwmg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gqdvrdfeb.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gjvkubafb.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gjjslwjvu.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gsjdsswdh.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gkyijymsf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/grewjudsj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gforwszcw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gzjvsxqoz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/grpyucxee.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gvhouglfo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ggatfcqzl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gnbpnjktn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/glheuxwcf.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gxpculrin.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gfvhnqbyc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gnhrvksmx.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gdotpqrrg.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gnjyomvls.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/guhbwtqgq.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/grkpufwaa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/glkyhmkaz.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gnuzvwsge.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/ggtqxurkr.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gkfcnbuxn.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gwmfzichy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gzhgjdliw.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gzccqlhvj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvfuzqvge.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gpovqdueq.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gxzneuuiw.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gnuhajnox.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gyknwklnk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gdtgraicj.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gmlwysbci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gineebqtw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwgdzvrgo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gbomrcxfy.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gigugekjs.sHtML


<!-- 参考信息 -->