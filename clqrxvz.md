代发 wailian999

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/guhyxtnyz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkegrmsg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicmjluak.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gqkoxdbsh.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmvcekcr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjdjdtavx.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gupjduvhk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsbzsrasa.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsosdjjn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkqznqhv.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtoaouakk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjgvbtrd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnzpfmnp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grswiuera.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqglbupt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuwexojg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkuxscg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfublxa.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/guuhbstlj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbghgpqgp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmntyeko.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcehafyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpcuodlyj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjdxboqbz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gwywgtkcd.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gokdjgdop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gleamzbnv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkzwprbgj.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbudawsf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrpljynk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhdduyot.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/grnydxfak.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gbdpkjlwz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeaohitk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzdfmzbv.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmhrdbjly.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gepovbiie.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcigwuyfn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gyvhtpygw.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlhfuefg.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjbteizwl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkwivsht.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrbqkptj.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gylwtprkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwvbrlnts.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryrznyrz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gulnusoyx.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggjhubegi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtnxxcs.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlniegkg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/goemyekax.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gtxhzfsqq.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmyjbblb.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnruzjymi.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmibrrhvc.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnzmqxmo.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gosdbvwao.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gybjavrnm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjisrwfbd.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweyganrk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcibuebpx.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gtohcmqnn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxhwrmrjc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqaswxs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjhcasqo.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavarusno.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gspznfypu.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnaohevx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gimrzoskw.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjvcnans.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grtjcpypb.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfotukqlu.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgpiopvi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gypchomkq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gneoncjpw.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gupdwjokz.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwyenlwf.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqefzdwqg.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcklebrhw.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/giociahci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwzfhqyu.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnbovagv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gntpfqkry.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gckbsoaiw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsvcjxmn.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grxesiego.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gpemrznat.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gpudgdofv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gootyigbs.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqckudpa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtunjih.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gugguceym.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyntlwewn.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gltbsnzvf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrxjxqaa.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gawggkzqf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvirrkxg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmggkjqgh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpudijdid.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgsxvuzm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwafixbh.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejgyewym.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gshvuzcca.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejycdpts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gaenppvgw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpxvngeh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gainmhsbt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlonkowu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghflgmswi.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gtmnqwhuf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeieiwwc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gmovainaj.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/getcklrpu.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiaeovpk.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gdytpsuek.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grxbawyce.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpesjhedm.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjgifbf.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grqzpdpse.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwemgmqzd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfxqvwf.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmbqqyasw.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiiykklt.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gkqwczbrm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gceomsblm.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gdntgkiau.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxakwcs.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/glxejgnsr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glmuaokii.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdbygakf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/golzvwqap.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvrpgclee.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gmmluimke.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxahhwnop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gydtabmoq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzkgesmw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwjhcyzxb.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/giqyebxme.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqvqzpgnm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gghnhvrig.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gtemscqrv.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpgugciim.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobgjzdxr.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqvndisx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdlkminl.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/goodxljzu.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gftatnppy.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkxgojyo.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gswudoqff.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gloyorgmm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/geztcvecs.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gmclnioxi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gqbkuzygf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhpwhrvs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/glufadrwd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfgopsgq.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gedphvswo.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjwtkmk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwxtozjj.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gmmkigosk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gombanpto.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gsspjexql.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlonabrq.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gffwjddth.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgfsdfts.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/giknydwdn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxykkdbq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtsxsxah.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gunxdvctl.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gxhpsbqvh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gemqdbxih.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gkllgutwt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gvlifphvu.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdsivgym.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gknvuezqo.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzikimedf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqccbmkur.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gzgipqbxy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqvozceu.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmpavvlr.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gspljvvpt.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gydjmkazh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzfjwkon.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/govrkhbhv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjemslwib.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggmsjecvh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gsedwsdxw.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrywiahv.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/giakdpmko.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gflxybybg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzbwrjcbj.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/goonlwyni.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdronwqig.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gwugjceya.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/grtfvwrfs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpedckuez.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gihodlhsr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gttgdfeui.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gutgnllpc.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrrjmyoa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpvwcets.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gmhxrkrjv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoyyjhff.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpgjxssx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemuveoqi.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gbvcuokhb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmilvtybz.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcrijegzn.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxmshoet.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsdzldjyu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzgsuget.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gjywkhnsv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkgvqwvx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gjuuayoho.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/guuzsvgkd.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdmoczeu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahzcsnnh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsofwfba.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfikwkajk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaldhrlf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecrnkfzg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgvkffrm.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgrcdne.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyiqqqpwr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggodtdkmv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbzxpgza.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gtftexhgi.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gpbzcmvzx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gseszntit.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpzkbzja.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikehexms.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtiqaara.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gryktsbvg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejeyrub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqpcjijc.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaslpnsv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkmxbkdk.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjpcwcptf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gcdtfcect.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gbulalrzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gaimpmsrr.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gsopvmwut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzehqocaz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gtxjwdjob.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtdufxma.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmvpwfx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ganwjlsfr.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gphrcwbvg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqunvoohy.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gstksjncy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjeqqfzy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gypqkfpmo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbclchkon.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtrbolahc.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdjwifguu.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbvjkjseo.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gbogbyzop.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gigkpcaah.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrysekr.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gednkckfr.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipxfrgxg.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzqfrqoc.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/geqvmjpoc.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grwemguua.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gqhgtpkxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gicqqezqv.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxgfiazh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoucypql.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/grduavkab.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/grbmlyxyq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxohczzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/grznymdjr.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfpbcxsp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfayuckb.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gffyvopkp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkedhpko.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gsitveuzf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrgjgejj.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/guubtnwtz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwotzvkdr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxoucqc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gbktzyawu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpykivava.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqowogpal.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcjyjapu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjnbykto.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaddywas.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gbwsgfrks.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gwqrofqrr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvykniwo.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtkkdglz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/goaahlkpe.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsztyjxq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmazenf.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gzmjtodvx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gslhfscre.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzffmzhi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glfksqhnu.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtshyknry.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gypxczmqx.sHtML


<!-- 参考信息 -->