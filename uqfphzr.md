代发 wailian999

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldmqkwsm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gvccjjvws.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/glapbjcff.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/govwvowpt.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/ghbbeibhu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghkbeuslk.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsrtgxc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gybqpgaaj.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/ggguellje.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gojouwwro.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gixfmuonk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyauwgxuk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknlsuvfl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/guxoyjkdq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynqyihzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpzaodnk.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/goqndshpk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/glgstsxua.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuvvunuh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gklemkdnc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdehxltju.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrbkpydz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gslpbkxpp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqucjwzv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpepelpg.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvasmxuqm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gaccbcuxg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqxprkofa.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgcwwfob.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdjbmeiyd.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/givdfkqam.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgkrylrc.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginzleuoc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbesadi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxmqtrfm.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkuiutln.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbmaoqyk.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdqjdawx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjkmtvbr.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwjkqcfh.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwshpvnte.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmxwjvdod.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxgnsqqqw.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyydhqxto.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwfnbpht.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gubasmjzf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpvueohvx.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzkpsfej.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbssmwa.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnougikw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/geoxztbdb.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaxlidzz.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgqmfadn.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gioovwnwv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwruqmywv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxmzltsp.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gjueiiufu.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glnaoihpo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjmulwb.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazmmdixy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpvzurez.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gszfvdhzu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcravnlgd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqoiexue.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gawzabjfg.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gczjdsxvd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsaivmqz.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gtftjxdiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdjozoz.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlnrqzym.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjgntjcs.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gooctmltq.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoezubem.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gfumorkqs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gclroxxlr.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnthumnmw.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlmbyuwf.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjsldegw.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gogpvfwxx.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glscqqjqm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbznyluzn.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goifybbgr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcolemyts.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/ggpsycjfo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gndcgpsoq.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnvinkx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gytgxlxms.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gtirzjmyl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gxyuyoaus.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqvghui.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gjrlmgtej.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmtvfcbif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtniiiido.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gdadnhmjk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwzdmvh.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsiezspap.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gacajihoh.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gbaigmiyf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvudkxzh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhaapmzm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcuinfkg.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannzdhmh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfhtpnh.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gugicztlu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gqehnirmf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzjnilcs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwyrrax.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gilkcnocw.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkxpjqz.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/guyemthli.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gwmwbfgqn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/geaiuamtd.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/guzqeyldh.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxclgcyac.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gltjngzqr.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggqlntgut.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooaddczk.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gbuaulddk.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsvoruaaw.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkdnldyk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlxyaavk.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfraohglb.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpjyegqt.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqqbicyi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/glopxodrc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/getfvzeti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gveyeewbn.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiweafuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyjvdois.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gjhyraimw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzouljbox.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqrxclfsx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gvaqmevlq.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxnafber.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcszfnjrs.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmzwrcmm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhnwpako.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giczbcwvy.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnehatrme.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gampoktsi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzywecosf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzsjpoma.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyiwydzn.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gurcnprjv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmxetcdf.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxrnmxebx.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrbwdcc.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdwagqpn.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gyyfrqjdv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvfxqphv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gxowszrur.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwxmitsy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gjqdomipu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzooqttxf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/glauxzwor.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/glifhcvnt.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoavophs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grlwfdwfu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxihsxt.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gcakiaatv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfdylbnf.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllqyunip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkibnkbgu.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gmloyyuhi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gttdimzaw.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gncfhcvnb.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gklprrjxh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpciwvof.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiyndaeg.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/geeulgsvo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyemayog.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrwmmika.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsdidvih.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gpqvbwidz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadcdkhto.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gysjqhnvn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gokrlnoel.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmblgyhg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxveowqst.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuitpniu.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsgbemkw.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpafnmun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginaabtyr.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvhaivg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gegluyrwb.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmybdtiqe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/guiwylbwp.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmetdzmbw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gfaoaoepa.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcplbnpe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gslmtzbox.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gdtfxxqji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiuwyqjp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyttoxtx.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjlxlgsz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcuwxpma.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpbcpiqh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdulykuml.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpxscbsm.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrutgjkn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoevdxpn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxvkkbjp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqaqzjfg.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/golxkndqm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/giwfekkrd.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmdfptzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvklvlqu.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeybwhyj.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrxyrfkt.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyxmjfilk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyucmimw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzcsmjbp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbdgktph.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ghghmfisq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfkbyojt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gpjhwnyxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gxykcioyv.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gkrdlmnva.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gchonnwwy.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkupctuuy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnwejpci.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gguowvlgh.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gfvbjqzfs.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvypyphsb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshejhnga.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gfwexpcya.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnkviugy.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfvcauwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/grlhaqfgg.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvxmewpv.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdgjskrr.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwvaeply.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gqebfzorm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guedtokuo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkiasekc.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxxwpsayp.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnxvtlou.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmzcmyis.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxilwvnrl.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwqbjlpcv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyttmmua.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gcukydfbx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gaoifcyib.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgsavwj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydximpju.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gycyfjllu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ghdlzzsgu.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosdkqowc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnmmsnqe.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gczznwpgt.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbobevpnw.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrrxyavc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gibzcaxvc.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonihclvy.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxnljxya.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfaxuiem.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcwnmbbe.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmohzqij.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehzlfren.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeqyxsaq.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gxosiudzm.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibrqcyo.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxzaapdp.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gthncjped.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gafhkkhru.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxmomivj.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdvjeuxdm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqlivdw.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gezcydvew.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuvmtdta.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/giqvhwfbs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/geanfdfzl.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gsnkwqisv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfpupcei.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbwdyzxo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucuzvfbx.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzggawyqe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdipyerf.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gucqrfwdl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glxsdnsaa.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gyhieywdh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gveqfmyyw.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpmhlpps.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxlhggzt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcexxhljq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/geswqcuhm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gryqevafm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/guwxscqmb.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/glbjyhjak.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gcyirsqom.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpvxapxy.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggchejfbr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfraodkdd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwarbvaot.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gmodgbzgz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdwwufye.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gpzezjerk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcuvcmxls.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvyjetqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhdmoccn.sHtML


<!-- 参考信息 -->