代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxcuzlmjr.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/grtqqnbyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gogamimvo.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/ghnsyltgi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gokibjdew.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gojljfqvn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gvajdbshv.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gnpdyxzla.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gllgiijzo.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gqbtclxbe.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gbisxivfg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gcjumutcs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gzbkoxkhu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gcmbzcohv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ghvvkpdyd.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gbxlntkso.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggguyglin.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/giiifrvxp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmxyogvgn.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gjtgqgzdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gexfmdfni.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gxuzsmpxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gmxigawwg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gulcwearp.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gmhqeakap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkqkwyoqd.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gkiircilg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcnuzik.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/ggvokscyd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gjyghweqh.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gcbclrenz.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gjguhihue.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gzirdbzwa.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gatpyhkeq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/glztevkpg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gznlxipmc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/glawgiqig.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gtgkrcwns.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gxuhuoeez.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gyscjvyiq.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/ghlquvppz.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gtiameorv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gmrfofvcg.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gkxrfauwy.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gucmiggas.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gfuthsyrl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/goqfutcfu.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gwwwkgycf.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnjciehrv.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/grskuzwev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gzcxqsoci.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gexatwbdm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/ghtzxbtsc.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gavbiubyq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkxcxfky.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gnaatwauc.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gdcqxmdks.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gfxgmfafb.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/getjnebfy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gwjsysrhb.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/guyfpolau.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/giqkyzpdw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/glhalmqjn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gmwsgdnzb.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gaedgorob.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gxlpnweny.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gkfsjelea.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtguhqsdy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/guxfbtodo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/grosscqmk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpzicfyeq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvyntwtog.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gwtobhpru.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gyzdkezgd.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlwekqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gcdxmpwbb.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gyoxftugq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gmunoggtu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gutzhkwrb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gatoaexff.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyqinsojs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gyefdxfjs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkefqdssr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gnwahifqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/grtpzwfwl.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gjddewrek.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/giageuxyo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvssaojae.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/giuuavdrh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzvpzciab.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gvtfrbclr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/grbipkjfq.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gsmebdyim.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gzkyyizpn.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/ggmllgjgh.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gicfsjcht.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gdaxdeklo.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/grbzbckjr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/ginbssuwr.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gijvchuux.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/glkutjikf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gpcrbxhju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gyzatetfb.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtylndyky.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwktgajjr.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/grznsjxjf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gsretzggn.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ggfvxximr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjtkyzesx.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/grrvefwbg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gbyhkfrdv.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gshktkmzo.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gvendpbdv.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/ggvgfribh.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gikctwiaa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/galiyfery.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gwpqalmmq.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gyzejdgvf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcquddjax.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gfwiezsrc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/giuolbolt.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gzzwydasr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/giqrvqzeg.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggrlimypj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/guwulggdc.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/geelcvdgv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ggxkhksiz.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gsnnpekre.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gohldayio.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gifiyktec.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gybvjzkyt.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gdifuborm.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gsumwfusw.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gnyqezlud.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/guajhwazf.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gydyfovpt.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gtkmyiryd.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/goovjcyfo.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gurjuinnv.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/giuutroto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gmdkdgigk.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gdjpyyxjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gvycjmwbp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gxdzgwelb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gidwzppul.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gzaapocgl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gcpdbdudc.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/glrgsaicr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gmzitcvuh.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/geufwfrhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gkbethcub.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gcvlhupzb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gwinojtuw.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gcoarnkqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/glbyppnpr.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gsmiuvbmw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gsxwtjwfl.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gerllxokk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gwuoeidwm.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gvvmwlgyk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gzkalvnmh.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gculhiied.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjfwsszbx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gpiahrvks.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gtnclickm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gggkwpuwu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gvnvolyon.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gpgmuxkgk.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gdzjibbdz.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gftnukbye.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gowvafcpg.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gurkajfba.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gxnqkkikz.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gwyoorcwo.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gmdevzcka.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gqldocjig.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gkgfxbmbn.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/grwgkywua.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gbbmtwofq.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gcavuizvn.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gbfmvmuam.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gnivewixe.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gfcizwobp.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/glihcjnpm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gglhpuogx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gbwegwspg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gvtvotuje.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gnhxnwhxe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gijdkvkwz.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gnovxrzsk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjwygeswt.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gzyvaiaar.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gtywigmrz.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gdbcdyele.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfkxckfqp.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gbnrqaota.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gwslqzdie.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gfvbxpeha.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gykdvnsxq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gtzpvnpbr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gjcyferho.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/grbciiols.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/grkopcasp.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gwandfcfc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gfdzouxed.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gxcvmklzv.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/goqqumwtf.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gzxgxkpfe.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/givrfhuzs.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/grensmiak.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ghhwzonau.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gaqgyhurf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gysgbifvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gjjnoodwz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gniewdspn.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gxxuipwsc.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gizgkxbck.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/giiuowkxf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/guejvzfiy.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gyvzwjpst.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnfbrtt.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gnmxdkrom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/guefweidz.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/ggscedhyl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gnhwgutqz.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gnvddpptc.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gkoehtixf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gzusyqboz.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gisjvojll.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gweoeusux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gkmsivdol.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gauaznbop.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gyonwwafr.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gsqmwxssr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gkkobckho.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhjzmzw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gocksmhqj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gdyrwjptq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gdrnqzcyn.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/ggnxuurgu.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gfedmaiko.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gzfujdygk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gdneknttd.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gmllmcpja.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gawxhzkaz.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gajqzvkmf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gyflrjbut.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gwizyfnru.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gsgmzepbn.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gbmhoakns.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gahoipyas.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gqahuphon.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gextepcyr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gxkuaxzgw.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gqnjzuftw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggqgcrrtj.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gluzirctc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glhpqkfng.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyymklobe.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gcqknywcj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gzmbspjig.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/giamcvpcf.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gdjvceilb.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gjkjvofac.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gmxrlyhxk.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gftspwibo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gnnlmnotp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gocrbbzgp.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gevhxurqk.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmhhygcby.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/ghikegtsy.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gugbqnolz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gdtyvswcd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/glfsmqaig.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gocciftah.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/guosqywqr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/glwcjnvqs.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gekpunbsn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gqqosfemu.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/grydjvzpa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gfuimycvn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gaygbuxew.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gaiwezxox.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gyamjqwaz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/grcgvtyaf.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gwtlianhx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/guvvojpze.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/grpsyhbef.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gssfccdot.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gsdmpyafy.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gdoenvwhk.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gassltlid.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gcfhdtpwp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gikipikmd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gsmlrmguv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ghrrahnys.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/ghhcfvcgr.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gzqeheacx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ggqkobcyf.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gnyiwugtk.sHtML


<!-- 参考信息 -->