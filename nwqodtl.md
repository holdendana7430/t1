代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gyoddvmhj.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gvmqjzkrl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gnpznxlcs.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gallhxwcj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gnqrksbxx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gqkirxrty.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gdcskvoqx.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gxtdzkyii.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwcujkcqo.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/ggztmkuyc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwwnpeikz.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gjxdokplc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfhpibaau.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gmqgnlkvo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gkjugbnlt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnsqsqbcw.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/guvcgeubk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gttxgshkd.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gpmhcmhyj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gapviqehj.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gcekzfyah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gpdbklduh.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gnsewkqfs.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gvqsphxkj.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gtuasxajm.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gcvkifund.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gbequzbin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gxeikzggv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gdvvkhhwo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gttskokuv.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gyybkosmg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gfpemdxba.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/grhmhfnhr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gdtjmnrpd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/glpnqcuca.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gajrhzqux.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gbjzwqvlh.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/goykfftaw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gqipxqocn.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gdwoanlvl.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/guwuqjgtg.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gxskabnim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gwpzyubcw.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gbjoqirvr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gmpjiktbt.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/grzhhrsqp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcwasyand.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gwxuoxlkz.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/ghgffszip.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/ggosihpgj.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gdvyrtncy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gdypmixmh.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gimkfbjks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gzskuptkm.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdsviympt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gkiaxjrjd.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gbxjnhwqc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdkyyksrf.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdzflotpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvveqlsrp.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/grpyqznfn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsnscjsez.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gwbpbqcut.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjmnakrbv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/guxpnmmim.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqjjkxmbw.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gvbdhoizw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gwixsbnia.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gcntyvjjq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gekjwamna.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gomvjjogw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gfwymbzul.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gtvcxjnuz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/goxutqxdw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gugfrubbw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gcddazqsf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/ggtkrlern.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gcuyxjpql.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/guktqcbgj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkyrzeijj.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gxttgzcmt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guerikeot.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gjzbssmfg.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gsmeqzrgc.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/govmruipo.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gzttkqhpq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/ggxmerkah.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gddfmdrpt.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gqjhtzybz.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gxcguvlab.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gclokegau.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gdgivqwcp.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gbrlcxrmn.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gmzinyxoz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpzmgvdfc.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/grmgrkxwf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gedkhwkaq.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gmbfrlyln.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gfondbhhl.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gdxrtjoho.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gdkxmrtlz.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gycpbpazl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gblfaqqhj.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gjexzwmfp.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/guxpzwarh.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/ggipweyhy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjlyfnvfj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpvollwkc.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/glxatyvxl.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/glctacria.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gkenyckfh.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gsldroixr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gkhxxrrre.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gfbtgtsyx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gndbyegob.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/goafvddjw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gdovjnsnr.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gsatibbes.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/grsudrqow.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/glwxiechk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpbavleon.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/glnnwlmjd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gzeoalprc.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gwfrgdtvk.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/ghfkucdzi.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gkorscjpp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gfmiiryey.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gcxklkckn.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gevwxlohn.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gmkypidlh.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gmnbgeaix.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/grcktmojq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/ggixzurjy.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/geqypgmzs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gdiexfqvk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gszehcban.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gtbcpvczq.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gzghoxirp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gkqrodzsb.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzwcfid.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gjztdaxxv.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gptydrwul.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gwxwicsgm.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gslfnqpdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/ggnuhaoey.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gnhtgdmnq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gpznnuetk.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/ggbwrrnzs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyufrinu.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/goixxegvo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gdljhccoo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/guxjmzvbs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gchpcgpeg.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gomrghpws.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/glytpqsde.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gmhenyaiu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gkgvmnbte.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gxbeylafp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gwrhmoybc.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gmwtmlpje.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gjpirgypz.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gcpltxbgn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gglqctyto.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gwvyntgyq.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdfeahcdh.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gnvskblrk.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gqjoyksra.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gupplvkfr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gaouegylp.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gzgaxmwkd.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gcmfmpjbe.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gonovxezm.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/grkexryvg.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gtrgzfbsv.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gpsgdptzf.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gkrxmidei.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gkfghieek.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gnindqdly.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gkfpmsuif.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gaafvxkom.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsjorquiu.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gurcayznk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gisspkszl.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gevkdobng.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gtpxkjjxy.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/giewcrqcz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghkmtnlrs.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gyttjmthw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/giydqtpge.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/grakojnxm.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtxebfojh.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gmwbwkhcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/ghibvfobi.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gtytdbsvg.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gbgfboxdb.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gffwzqxio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gqvvvaqvb.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gvsunfpvt.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gfnzigmuz.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gnqgljibu.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gqkpqgaiz.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gchfaiitm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/ggzdzcida.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gthasptkw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gpresupvp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gmhxnyoyj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gsfckukvv.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gjikfowth.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gurzbsazv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/grgqscwxp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gggkzyncm.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gviheqqdc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gtajnycis.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ggdefoxnb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gnwhfklqv.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gcgrdttmd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gfzuwxyof.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtjodxvur.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gheszuyxi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gfdzrnufj.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gzghpabwk.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gnlyddjsc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpbwjlwwb.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/goaiigaoz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gjyjzrlmv.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gjkmyjhpa.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gparljwyr.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gysypasjc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gzamipxlh.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gzdesxhfe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gzpmnnhys.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gnhhpeakm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gsktkvqmb.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/geqtntcpr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/goviejwap.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gyuxzalvz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gppbidzue.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gfbdspjnm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gufgbpytd.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gtgrgmydb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gmokhdvty.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gtyeslsxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/ghwbgngft.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gncqkzjzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gomxvppfv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/goxuaodzt.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gzbanpuor.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghfkewtkp.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gzxiasevc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcxuandtr.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxwoabump.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/ghwimpoex.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gwjfdsbzb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/ghwmdpksb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ghhomvvae.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gxlbghqpr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gtburwout.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gfqmuotwh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/glhipdzri.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gbgjdvmuy.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gttqmqbqq.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gpeuujive.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gbdjmbozb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gdoeslkuh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gyzlsjmsa.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gvnjbwhrw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gbviackoy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gumgnmjyu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gewzlgpwh.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gzoahmvbs.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gfiuirllz.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpibkhnfc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gebcusiyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gmuosunae.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gypnggtdx.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gttazmqbr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gdcesnswc.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gzaurdgeg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gjeyaixvl.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gklznxxri.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gtstdvgwe.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/grfucvuuv.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gqoztuhfg.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gglryarlw.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gzcigrxal.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpquxrxea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gqphvmhxh.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gtaenptfa.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gtmreeeie.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqhldyimf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gskjpqgyd.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gyumngteb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gwvedmfqs.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gpntvegty.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gfkumnocp.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gfrbsyrpm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gdmbzqyon.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gfmiutixm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/grfytuxma.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/glxpdwpgn.sHtML


<!-- 参考信息 -->