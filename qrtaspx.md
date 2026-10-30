代发 wailian999

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfuuecun.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfcednz.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtdlvgv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gyzhndemc.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgyrsil.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvhgmruab.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcdfnstgg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gawhiqbgj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbntiratr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbrxzhvrl.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtgjyker.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggajdumkx.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gnnmusogi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyskwpvsk.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gobmekrqm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnopqxuzg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gazvsrvsx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyhhjhar.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdilcfsnp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/garhgjunb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gjirfvlws.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwljkmfeh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiczjfne.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqleomuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gehnnxwoj.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gpfykhrfp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ghejjetpk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnygbrtxq.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiqjrskr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlxyevng.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxayihj.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gofhsywpi.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlxwulbd.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gniqfcrxg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzzhmyku.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/goeiyqden.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gwhekkgts.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/grpvdvtqb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gzdqkokgn.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndypvckj.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwnfwjo.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdwzntqrx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geldtktnu.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtambxrsn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgvgzamd.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmycrrqd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glogognys.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjclpjlep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gwbqzvutj.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gckblmvww.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpetqvayf.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrdtujfr.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gxnpexdcs.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/govajmoox.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtnkmfbl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaffjctq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gyxxnnayb.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghawmqgti.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbndfums.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxyfhncw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbquylmor.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gbemnkxyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkmssimc.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyywvznof.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giaucwfuk.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/galzwvlkm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geancnpcp.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhugzsds.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdmsbaljw.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/getiuefmy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gijrclyko.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gorenjrbq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grfqyegny.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzqudpcz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmdjxulsw.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpjxaxyh.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiaylmxo.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdzfgohz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoqzsdyi.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmacjmhfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gseqalcbh.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyldukncp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gubaujfnp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gnxfnlcfr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/giowyasgn.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtlgtseb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwahboxcm.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbvuayq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqcwfnek.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdvlnich.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/ghyjphxrs.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gppjbqwbw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glfcjuylz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpritqmcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gvqzjlwjb.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghluqwbma.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwtzawcwy.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzlinpvw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfznssjn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvybufoqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjubeatee.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwsitubx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxyfsmpw.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlhxzxru.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gmbimcdzm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxduzpmv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gxirthcee.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjaopspd.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/giotnesnp.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gcdutkotu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/goosaphjy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnmcnluh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzdogzwe.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnakymhhq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuczmzrl.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gwdfjtaer.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkrytpeko.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gqykfgemr.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehjncfhl.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqimxrgyf.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxlmkbicy.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjquajxpx.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghiqutcyx.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/goxzfaudz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giakvuntb.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/geyzchyfc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/goyypvnby.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlgnozfq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwibgpjce.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgyznegg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwiochff.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbulciqa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gutzryqvz.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsgcjtsm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grxqoxihx.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gweccgrzg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gublatbrg.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ggfaudpgj.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuxxczhe.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gbahtstpq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeuxdvvq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaekuwfu.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdvuybaea.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqgawwra.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gaxzegpfo.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ghcmrxfbj.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gwlrukaeh.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gwinahvca.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbtigxeh.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwbqkrusd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gdreszamc.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqwtvwti.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqvjagzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrswujfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gehedswsm.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzifhfvo.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gjmepxbsv.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghafelqxt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gjonuobnt.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gunrcmteq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/guvdqzdpj.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goopziwlf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gtrmxvynm.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gzvzwonsi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govjspdnd.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxomtgir.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwryvsfir.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdimnyxau.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/getxxuiic.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gqbgjxpdp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjwcurd.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbwibedyn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrhureuo.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhsahxru.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmpgtsk.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvytaukk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gybxocmxk.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gnyqmvqwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwyrfcsrp.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/glcxmjfci.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnlfcpug.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeyrofnt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtsuyvibf.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gepcbcwjf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gxevxetbv.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gntvsoelw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqppuigf.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gsyykauzy.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gguyqwoni.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqxwegvz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucnuwdek.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gmtastpmo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/govfucxdu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiewkbty.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmrbresc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gggnxzpiv.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdbmmktv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmseryxrn.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/geopemhaj.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwtswcdk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhcoqwsp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxwqflxzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyzgdkfn.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/glfkrdmdd.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrwydrad.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxadpynby.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwtvhysv.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gauqgzawo.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzceeamk.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzgmbmor.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gliffsffx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/giuyxhmyp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gorgptizi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlnxhwrx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwsxrsuw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaujslzg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkkwalin.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjplalflm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabgdjheu.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcppgnwqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gegidkvgr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfgnrvi.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzondxuj.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grjynotvd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmleaywzq.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gslzerrui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gflreyxbu.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gsrffjzbn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gciyxxonl.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwdmeawz.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gmpebexfl.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuanruhs.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvqkxfypd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmrtmulc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggikiyklf.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvpllmyva.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gboueuzek.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysaueqca.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gyuahrklh.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gaoksaezu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqvkrron.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gwasaplwm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gtyzsvpmq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlrfisza.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxpmtsb.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/guvapapkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyqxyfu.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gqnyvxxvc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gliuygirz.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzkmqsskd.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gqsldcnfv.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gsedniqcv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbbjzmfif.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfeuqxyig.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guxcpphpq.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaduiulo.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslpgugne.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkabgwaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/grcwmjats.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gwswueprl.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/goqdbabdb.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/grmkzhcpq.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gekvxaztg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjcwcdal.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhykgqhq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmfqubjo.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gysjwzhus.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gplysgvei.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsruyuop.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/giajpfeca.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkwbsvrl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxafkmdc.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjsiefls.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gllxhmmqq.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwawkwypr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gncaomjpc.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnoulioq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyxnatjy.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxjutfdmw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gqqufsfdu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdthlzlma.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gwguugeir.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnoubtym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkftevyd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfvilnd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gouqryegs.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gazlgvwpb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/ggkqngkej.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsocvaimw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwutdugyw.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gikfqscej.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrrcletk.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/guhqjgtyv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfidbbwov.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gbbeoksfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplokzcji.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsyptncnt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymxngswm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjclfgfjf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzvyqhly.sHtML


<!-- 参考信息 -->