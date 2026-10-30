代发 wailian999

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/geykeighf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gasebooar.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/grazcgcle.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gllcjubhp.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggscppyjl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gxcygdmxv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkifhwwwn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxfgtvmm.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gipunycos.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqkbusnu.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyllljebg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gblnafxie.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/giobwlqya.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkinmxgzv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjpcfvyh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfflnrxn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgeamjdg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejikfuhi.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagbgxgz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtqwojrd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gdgoyubra.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gpugiigty.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnabscii.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjlbsjcl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyfkihwt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gluphzwjp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gruvmjmcp.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpxrlaxag.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbucgknb.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gariispwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gftlndnou.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gifjidlks.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gdywsqfll.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjoxvjuh.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gqizxynis.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiqyevum.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gfotuxkkn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzngrjzsx.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnwsddwo.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkbnraegc.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gdohqiwqb.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzvshwac.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/goafzjqik.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwouxhebx.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/graccxxkb.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqdnmntql.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gftwwjqoo.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgisxmfc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gakdlbtie.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtymptnpu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqzjcgqq.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gshwujyfe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjtaywdg.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gefdhcadw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gnvshnukj.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnsyswor.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsulmohxm.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuznvetw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfxpcls.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvfyshsv.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzmppow.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdnxqusuf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaxrdavr.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghjcafzgc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjshfwgdz.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabkgamrh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gybapbgkr.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcovfxmjr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmchinoow.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvfywswqt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwdjwwcib.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gbrcbatri.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzrhhgmji.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gplymoxmz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfnbvadj.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuwzhhpc.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glnguvqdp.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gklrzixqx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjnwhsnw.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutcocpkf.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcflnkuoq.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwaibtzw.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsagjisk.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcamaejxj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmokrbqlv.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqvoudkmm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvcnifqy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gokryqtxz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grwggxwgt.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gllmaoxcf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/giarffrle.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gioznlxnu.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gvbufqmsz.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/getoqllxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/glgroryqb.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoaljhun.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqqivjjl.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gcvtruwhp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsgmdkyk.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzibscqzq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnagodqbo.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdsetugs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwrsiudst.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsipjeiw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/guepdasyr.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpazzniaa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gocoknevi.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gzectligx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzyzfsum.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyinoelzb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gzwljcnms.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginecxqvk.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gomlvyszn.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrweyzgg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gbotyiehq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcmjkplr.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrvpyrq.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazqmfigi.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsquwhbod.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjutelvy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyveujlt.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxecaxt.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhujbyeq.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvbuggbe.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrypsbjy.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/guondpcao.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gedswubmi.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gqixropts.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gegdggqoy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gclowourx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcemvvhg.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsgjfymsq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjsttwnaj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncsrjnun.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbmvyfao.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaizazeb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtiyiagm.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/glguodcbf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwrcbstl.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdgghtqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/glpwksizt.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtufiekoe.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gswejvpwp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnszztl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvneddhnw.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkdfvqsni.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtynetdo.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesagcuyc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gbutdoahk.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcgsletgm.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gexatyclk.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/grtexsjaw.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvggqzpsb.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyxevftw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gyypwravu.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gudgeyjef.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/govxhrdzn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzkfyfwch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoxptzfh.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gbaauoxer.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaslptzd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzecsgkz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/glzrvlkxw.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsoztjeh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/glyrnzsfw.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ggnnckpse.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gxxlzlslp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guowassxo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnuhnzus.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdqvplifq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzhxcxog.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gkuevbwhs.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzudeklmv.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gqnjmnprg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvqigcgu.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxbjnxf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gthbtjlev.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkqfbnj.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywgrszmr.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gutefpmeb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwzsympvf.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpftikic.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gztjhkspc.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmgvookd.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjcazsxu.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gkegpzzhl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbagcksqd.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdernjitm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/grdupgzme.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwnmfxtwi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwbcwqrd.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gevvxbxct.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gnyepuajw.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gawtojcsz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gafsqnsgt.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gammtokrx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpdgnqkkv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gwmrylqnf.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawixunde.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnufsxbf.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvswylxty.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaamkddco.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuikpcjx.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gqjidoblb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghvgfqwne.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gugdjogyx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/goumcakfo.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrrfcaqn.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gzhipanud.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqudtbzp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctgtyzn.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gevfqhzbn.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxolrpois.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuftajot.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgftmhrd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfzukcjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gmkrmamxj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gwszgkjiv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxswnimiu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gnjocoqev.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbklucay.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gipavudjd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaywktiii.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grqnrbzmd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpqwrrig.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyanedqxm.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgoorqzh.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzceslhbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxpqsogs.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/giyqlgzfj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiedxpfb.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfonxevvn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gwztnldxh.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gftadlwtu.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/ghssvhpfn.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gacfpyugm.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbvqdxjcg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glpnazhba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gnwkvpphb.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbucfnbrj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnquaecz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtitlimzc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwmmznqi.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gustktayh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gyksivwla.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gvqwggsov.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpygogfnj.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gapcxiabg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gekxzxbvy.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvnzrjy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gzyafvxcn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbjnozzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofpdakpz.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gztolmyji.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqdgdpyg.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvecjqaqr.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahycuolt.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gykexnikd.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjthxjiwh.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhppsjgv.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkatsvbf.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzenqftx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gukxcnjmz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmtixpeh.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gadpxpsui.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwfgovq.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gowokhlaa.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgkshnmp.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ggybbqlpq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glqcpsjps.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grysapwmg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/ghwwozzdl.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gwldcdxov.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbhstbck.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbhlfgk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgcjzbbg.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gbulovzrp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gncpronci.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gykdvpbff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ginucdwgs.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/girxmsnhg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gskeprmpy.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqejnhyis.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmzhrsbj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmaebinp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/grrkbjzke.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdsbagzi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gcxkxzprv.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/grkxbkqyn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gptltcuuv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfvvjyml.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjevtloo.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhbtngnk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagghjzbp.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmurgvhr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpvzrwmr.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmageszi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvjtcnyo.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/glrbsteph.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goczcomzz.sHtML


<!-- 参考信息 -->