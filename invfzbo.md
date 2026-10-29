代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gzpnnssfz.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gquqzkbco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gvuozyxhc.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/ggntzklqe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpoioirls.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gnwzrfcue.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gxlfkgsdc.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gytmvrtcc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gyvgyzbmg.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/ghpeipbid.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnqqxxsgw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gnlyqooth.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gzfvapsqk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gjrmsidac.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gyimpinrm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gnhessitx.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/ginanhqdj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gpqaqzuvy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gnycykfwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gykejwdfj.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gomekxkzf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/genwikrss.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gitlnqkbv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsdrvmtvm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gekvjtumj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyursvblt.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gaebreaag.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmpcepmtj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gpqsrxpyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gstybudua.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gfoqclrub.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/giwsgdxdc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gasyvzdsy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gqhnsysrr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gqejnhsdw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gihshuhdq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfatfhcss.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gqxqgeflc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyatpfsxq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gaokczuiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/ggypaozxk.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gzotdybhb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/grvumgztx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtlyuyqzl.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gtnkfhviq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnpkqzmmp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gdmqgwvmn.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/ghdzeizih.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gmidnuabv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/geodvxgdu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtbsmyz.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gtxxfsxna.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gzwqcnorx.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gevmagazh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gndsqumpf.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gfdrzbdlu.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gtucimiek.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gxtrukvih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ggfhkpvrq.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gagiaebpi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gopmjxdmt.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/giyjrisyx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gybjnzdsl.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gvjcypuni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gnfdadslu.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gxkzfxoet.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gvzmjpwkx.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gkfcpjpqg.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gzkhszqgc.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gdwmrdpoe.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/geodxtnsx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/geikpemuv.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/giedtdobi.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gjwyswsea.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gdleqerpi.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/govlnkjhg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/glmfdejma.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gjukjaxvw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ghelmmyvb.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gezjdjqpt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfenjsfhn.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gzrobefro.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkqvtfovd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gntobbizm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gxsxtmktm.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gkkjnfdme.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/ggnfrdreq.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gnfgteedg.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/grqhxtfzb.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gxzzutthq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gsgtfdncm.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gygrgoyxk.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gtjohwdqk.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gyywidznq.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/grlwzqgli.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gkwiworbs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gafisrftl.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gbzfoxytv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/goudkbieq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/grxnlhnax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gmrlyipen.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gvfsdwbps.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/grtzvbqrr.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/glyawckoy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gnuetnkwu.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gjbeptbmi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gdwnqoqzp.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gdilfvojs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gktjqqspu.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gfrurgsmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gzlxieihg.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gtwonmkws.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzyysrgo.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gkadvhltf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gyrhsoybz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/ggxemvkie.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gsckocrdn.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gqylgoefq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gwrzcgwlo.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gmjyjbnbf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gxmnolrmh.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gphqxvguo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gvpakpxcd.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gcogrewiw.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gyuxmqjea.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gxlnckfjv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gljobvcir.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/glssujqqd.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/glpflmsnb.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gdqhcmwdl.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/ghljvfdze.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gesakagsb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gnzmuudrq.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gydozlito.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gvlacbkda.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/govrhisve.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gonrzchcz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gmgtnyzmj.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gqejfamfw.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/godpthbdm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gmznossxg.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gzsfuaaks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gkikjqphf.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gfzncskwg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gjrlxzerm.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gntjnpajf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/grltuyfsz.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gzczzplur.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gebqpgkvm.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/grxviqzcf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjzbfftkj.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gxcevinqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gljvxfwlx.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gbhxqihzu.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzpilmjpu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gunpjfjwb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gshsjfkfz.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gwcfpwusy.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/guqarewnb.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gazqtaqoc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gtmzxagux.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gjxswhorv.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gmjhogxib.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gestjqjde.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gnrtfxwuq.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gxrgslqnb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gdnroclul.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjctiyyso.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gwljbjasw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gcflmkwrl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gozvhvtth.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gvwjhsoub.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gouwxhxos.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gfxpaiwbz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gjzcxzgvz.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/grzouhsgi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gmcdiqnid.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gxylewkdi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gsgjgozoi.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gsixwzxwf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gtegihmbq.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxnxqceua.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gahyapqus.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gttzxelii.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/ghuoedumf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gxspjkhqs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gnvnauuvq.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gpyqhosfr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gfyeactvl.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gtqlucttk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gbigivgnu.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gatobrtwg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gujwmtzhi.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gegolrbmh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfzxpodbd.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/grajstsld.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gzqyknsug.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/ghcyxsdbr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gjkxzxlbk.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gortlhact.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/govapnssj.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gtiixsxwq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gxkuybskk.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/girxoyxxt.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gvbcrbhhh.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gywbrpdnm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gwwsoddca.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gedyrpfne.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqjnvzl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gihlmaqzf.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gxklrvmnu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghurjjmrd.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gjrrjiczn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqtekhvxc.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grrhvquuh.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/ghsovgmoa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gnpbbdoas.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gkakynrna.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gdaqhvykh.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gnaztbray.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/golgfszfb.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gpbgknlau.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gfagauxqb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxgnkpwrc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gmrylimbz.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gtnkwyvku.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcmbgnugc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gtgxixkuj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/goroibepl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gbjskotxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gfhdaogua.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gzeghxhto.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/guwemkari.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gepxyhcfr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/ggjnshvub.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glgufkpay.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gkqgzsdsz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gqcwqzxgx.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gjnnrbssl.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gjatmynul.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gecbgxabc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gdbhlgohm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gxapnmomr.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfyqwmneu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gzfytlqeh.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gvbhildks.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/grjpnwkua.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gfopmgcrk.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/glveyrisa.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gwuughvky.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gxpzfctbu.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gssebazof.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gaybkouin.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gysjmvbrv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwzntmhby.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gfrmfokku.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gopwyvphs.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gppduyedo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/grosgsijp.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gwymnmznt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gikelhhcc.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gtbgiqmon.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gcrppeyux.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gnmzqyybi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gjpnrxipm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gqadpnvph.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gpmikonyy.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gbscrmpmm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjkvnzgha.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gqiajvccj.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbluvotcg.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gdhhtifiz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gbrhsvypo.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gsscjramo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ghitqrafk.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/geqrqbsmy.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gznwgpxug.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gbyymdhga.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/ggejyrfcj.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gojssfndb.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gbbbomaid.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gdmfmszsd.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gbnpwjnbo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gwwyujpxl.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gklkqdxff.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/girbdothd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gytgpykcc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gyoadsppy.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gbbdkasin.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gioagzvlu.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gdubmgbuh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gkbsgijfm.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gsunefape.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gijlxbyhl.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/geukzuilp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gxfiumyrc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gdpxbalqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gmoqvhgcm.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gihusxyfh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gpvgkorle.sHtML


<!-- 参考信息 -->