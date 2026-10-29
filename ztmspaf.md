代发 wailian999

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/glmvkotlm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gexawqpbn.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/ggeyzofsm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gdyqzqcfu.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gaoiizliz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gnqyenglw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gsfthrdni.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/goiytvizw.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/grjvybfxr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/guetujcje.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/grouksxjc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnpedhmtc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gsicxiilo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gekhxztij.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gzalztzgy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwijmfrwa.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gswufvaou.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggkrraifo.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gjlquxuds.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gqfadrpzx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gfsujkurp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gebwlckud.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gsmernmzh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/geyjgkukl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gbewxgcfz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gnsgwxwog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gegjmfiyy.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gpgexsbhh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gqhvupije.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gafgvnxlx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gamtcolma.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyuttfmyy.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gdexmmrtj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gukiygpdu.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gorrykoju.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gtqlftaji.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gnvnbiknr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gpwjhyaic.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/geksdiqda.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gussoussd.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gnwavlgtz.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gtfhifwoi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gcsolcqnd.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/grzoqvxmu.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gofenvspn.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gyzwjecym.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gnoawnqma.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gjpxwxplw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/geldjavjk.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/geabqvsbx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gruoueofj.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/geaznjain.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gyouxhugy.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyamacjcy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqapanqiv.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gzzdevink.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gyjvxvpua.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gomqorxsn.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gpqoqjgfg.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gawevockh.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gthhmwbcb.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gosjtdunc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyuebdoae.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gvzuextma.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gmymbiaaq.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gxehhulut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gezndvura.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxnorkblh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gemmmxcrv.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gvennbpev.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ghqhavkyr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gtwhrxueh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gbtozhybf.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gulsmlevf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gglwiomnl.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gupvgatpt.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gyqeibcgy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gvdlwrxkz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gfeeevkjm.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gcfroyuin.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gyjweudpc.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gexrrptrk.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gdhprhhcj.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gsvudjwra.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gddluljky.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/ggvdjnjmj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gpggfptey.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gudexhgjr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gyfgxcoqk.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gbfdlxtgl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gyikkyeny.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gwoyyjmne.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gyrnmmmfv.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gidmtkcrp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gtmstjhhf.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gejqrjute.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/ghasvgxdx.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/ghpwviavu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gwlyepdej.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gddhifiya.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gxreurowy.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/goczgqebq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gebklqeha.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gzqiwjtgq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gdkonvzdl.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gxdzfgrme.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gpvuqvyjo.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gpwhvsydr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gddqoysds.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gjmuteiin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/grjsapgkv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gjxgedhav.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gzysaiefn.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gpecqzjnj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gnonxoxgb.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gkcxlhswe.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gupfnyhnc.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/ggshkreou.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gxfxpavci.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gfzjkcdbg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggyklgqly.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gynsozegt.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqjqvvefa.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gzzlzwabm.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gashuqitm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gsooefyfq.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gqobscwyr.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/giyixfrfo.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/ganimbpvc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gyumfuigr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gpdteyyuh.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gfiouxnwy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmzktcumm.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gfrlnztti.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvrdlenzh.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gguexenct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gbibsrauq.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gxjgaaorz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gjrvkwkaf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/grykqzovk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gwzdxflli.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gqbtglnhd.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gfikytyti.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gypxkltij.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gshdkmfjd.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/glotcahzz.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gsljqgksr.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gqvtljhdo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gzgokebcy.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gsdekvzqg.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/ghvqnltyu.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gxvhuafgh.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gthagprwm.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gbuiuhmni.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gzydsygnt.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gpcgxsyfy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gfenwbqov.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gtcmzrhwo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gxupdmail.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gsjvrnsda.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gnfzmuoab.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gfjrfodjo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gjdfbafak.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gbxxzzstv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/ghlddlpha.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gazcjzgcq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gvxomgtcl.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gdwxutctr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gwobxxksf.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gwlahgrhk.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gdpltmles.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gcpkznuvs.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/ghxseairq.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gjljworil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbyxotsjf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gxvycglfu.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gezannevm.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gqzpiupay.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gxodhngaf.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/googwnxdv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gpmpgnjqw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gyajwhpnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gvjoginyf.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gxzbeneht.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gpjjeteed.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gqdbyhwta.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gmawqvqvn.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/ggaoqpoxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gphpiirdb.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gcvoswrnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ghttanjtm.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gjxrfbuqs.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gukmzipuu.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gspefhyxt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gywpxuyfh.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gsojfsbfn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gioigvtfz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gjfryvkng.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gxlsvwnux.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnibsyjns.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gmjlgxjcg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gimmdvwnr.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfyoefhuu.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gskhdpmcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gwwdaxeqi.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gtupsnvde.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gdnbhrxgf.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gfcsmeldu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gdgrhibni.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ghvccncxx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gitnvnaxn.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gffmxahiq.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gaebdkkkl.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gripvyspo.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gvayhiajf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/geyhrcnbg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gwlvskjbp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/guhrutuox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/geyaiykof.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gzqmlzlbr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gkxqkoatg.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gaxmoinln.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gkxzxwduw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gbzqfvgdk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gkqlfisqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gctqpmrcw.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gkxwrulhy.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gobcjlnbl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gtmfzrvxb.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gbouwfjog.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gumyfpstp.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gvpymlyht.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gzduoyalu.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gaanxidaw.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gmatgowhg.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gkarjikkm.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gakrlkgjx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxfqvwraq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gijpfsnag.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gytmmfpqg.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gxnyvufqy.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/guqgkbkzq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ggilkovfz.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gaxkzkguh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/ghfgbpcbw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gyjtartay.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gwahjyqvv.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gnlhtrfjn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/grgiklnsy.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gfvdbuisb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gnzahuuvc.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gzgwaxcgl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gzsmasolq.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gkhqaovwz.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gnexxznkl.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/giicbmkfs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gprqdnmam.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ghvyeuvdi.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkbdeqvel.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gaupkihrz.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gktzlnmnm.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gejbffilz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gxlisyaqe.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gaeimtmqz.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/ggmmgzoox.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gezyzzsey.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gzximkuqq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjmjvmuwe.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gokdhoxek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/ggxxytklk.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gjehmonvm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghysycrol.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/guhjqrdhq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gezrfktlp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gzzhjzgoa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gnsmuqkqt.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gfpvqfkyr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxtzlicio.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gkydwkmvv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gnploanhv.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gfuimixco.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/grridypdt.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gxrfkooei.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkastjngn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gtiepydei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gjmnyykze.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gxtyxulij.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gvnzputsb.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gspekcnpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gxxffnrkk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gppsgtvii.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gfovxfnzo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gspwonfgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/guqyoingx.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gsahjpqrf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gieuhgyfw.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gonddbcvz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gcychxusm.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/grrlpvdkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gfocamchl.sHtML


<!-- 参考信息 -->