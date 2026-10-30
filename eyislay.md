代发 wailian999

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gerenygky.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giukecvou.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfbkpvffa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaiprcts.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxzlffbd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaydulud.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbolbblv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaspcpbo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxkvfzxr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytotzcb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gugaiatev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gkjwahvwe.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gqdgniswy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjubuydwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gilrrrkqt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grocamlvb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gbzvnebnx.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcmgyocz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdoyzmqq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtierxysj.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxstxqpu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrsqcsgm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbrxhzmc.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtovxsf.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtgwrntd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhdlaaps.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnczwwmwo.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvjdfea.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gkctviugq.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwafwdywe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsqaouwr.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuvbikar.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/godsoclta.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gliuszfwj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxavognft.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpejnlyrp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkohcbosq.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsihjrcid.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjjolvkk.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gexuggzwf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/glrglrnuk.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gofnkzgrv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfttdgcml.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/glowgoztn.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysoevagl.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztfvknit.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnytyosup.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobubdtsn.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gisseidmc.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gznrtqqah.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/galvghcze.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgxhssnm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqteomvnp.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvvgxhiz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/govxtmlce.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsrqrbgy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzomengdj.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gldduvyxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlhmyjpb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdasmqlh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdcgonld.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsrijnxk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvafzjkmx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/guzvwlvid.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnfhyarpy.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gwlqkymxr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghspzioqo.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkziyhijb.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtnmplvh.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkqkjpnx.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcjnmgwrn.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsiozgk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnppngmlc.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzrpudmc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhkkjfwj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gjnybpqlq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/giqquqqkx.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjtsxnmtv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqqezyax.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkalygrcj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkvvgxvw.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnbopnhu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gmnivldlb.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzavzhyye.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/goonylltu.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfgaymrwd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmclqipf.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzhekuvl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfqalkhzg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmunpftq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbjsthye.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbguctjv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaiexmsd.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gqvrzkmfp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/geqgcukxd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqhgohl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqvzmjoq.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gqxdcfufp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocvbvsfa.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzlaehymq.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/genviqkkh.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvfvenha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkvywnpr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grzmijred.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbenrajz.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gjesxxjeo.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyrkbsvp.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcimqeqw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqydwekig.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdjwjfiv.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqymgblqu.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdaxxdrw.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gyeyybbif.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gecpmxkzn.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdceijkvb.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjqlwwofo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnytzray.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ghccmobru.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gffgzhuzq.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxtlfcq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghrbjwvsp.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghedqxhvg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtqanlqbx.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gynmytuye.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwqbuzse.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpahoarl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gghsfruan.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxesuvf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gimkamvhd.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gunwgjigw.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzxobawe.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gsujeioni.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmlbqxt.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxncouzs.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzbbatrd.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gluslxlek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwbfvxku.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grrxjuuzt.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gkgykeogo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczfbugtf.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/golgbfjfu.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrxyzqw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gmdrtlgit.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdkkmqrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gnljsfdfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhwptbkp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gommfguzb.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ghyonfkiy.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gntosikdv.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gukrtufue.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gdbmbslqi.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gxeutfoqk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gzxhwxddo.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gesybgknt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvypbbaps.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxpknzqi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkfjltke.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gmatuokmp.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmlqgpqw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbjmyfdj.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbmwuzwj.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/geyjkzzja.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeyallgu.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gieunfglu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gbqkbocry.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeylflko.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvmuknoi.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gvollaavi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbtyxqnv.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gacproayd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzianhfpe.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/geokryacc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupjtioio.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gzrhlqznu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gardfzhya.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnadvjbua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gcipkfjia.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzbcevyx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtubjmzzb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzndjxim.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvsxewtn.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlwfjhok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gupljxlun.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjvqbil.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpjnejyuf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzitkvtg.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gzigmiood.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrfxerpv.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gslsmhnri.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvinvwr.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcdozgpeg.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gdzbleusn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwtwwidp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlipwmdw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkwrdupop.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwzyzdsfs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqslwzwl.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gyblcwqyx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvjdmqtn.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gsjaqlqit.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghctmvvpn.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaalqgie.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqwdbktb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqblzuth.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvzmlaeap.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gkytdxgkz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gunlxnrtw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiqpjcgb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gntqazgxc.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gefsdypvh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gucdfiqsr.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gejazehwm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giazseoez.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbrheeta.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxflunvpe.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjitloekz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgfvdmhk.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvktlsgz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjggbltq.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glwplqvjy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/grqxeuslt.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmazsktk.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiqwnazl.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gliqefxgm.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbovdjwz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkzjqjrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gtakvkllc.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbozirtse.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxovkvqn.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggpvthgzp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqrhrpyrm.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grhhdelmb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnsxgzcq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/guqrjgkpy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwfjyjlu.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnehwkqjg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gelaetrtv.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlwhyxzk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvtsnrpr.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjsahvzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycdttwee.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gupmmubtu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpihmonj.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/glqgjgzps.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezcgshzh.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gknwmwhvk.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guocxlqgr.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnlfmqcf.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/geovszyib.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkyzljfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfturkudb.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakceqdeg.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsxagzxu.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gclyxxuef.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzzfwmurv.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsuicetom.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gtebilcuc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geytnknxf.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmsiknxhc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdltsnklh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gewdzepzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gljwnvnkg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwqbtecz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gklratrvo.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gzgwzofcs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwslkuidf.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gtfehsimg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuaqgeao.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/givsijybh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gfdwmonjo.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkevqdrv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gutdsbtqm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdhpclmm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobymdzkd.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxfafmtft.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfrswdhc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfekwotac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxshdfol.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glyfomfwg.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gyweqiknm.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gevburfmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviyikmpu.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gsbdtojex.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamawwnp.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gldeevohf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfutxfen.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwmyrdol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqdbchlx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsvcgzhsk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkmabtwrf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzoaxwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gskuvapbs.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbobcaabg.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gziarajya.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewtiioep.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gigmedroq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glsuqdegg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtzunybl.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgwwasma.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gngsiuyzm.sHtML


<!-- 参考信息 -->