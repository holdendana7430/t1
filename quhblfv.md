代发 wailian999

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwszgrjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcfmnplh.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwmtaeog.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggzzpikdh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gsaucvcup.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrwrszws.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gbhwokchn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gaphksidl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gewgspfft.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdqmjyy.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahkzuzpj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/grckqttpf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gfastrwso.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gpredcxic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggucvsbbl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gogdcjasx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxlvraip.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gqwutmtih.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtmanic.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjebwscai.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gmtiascai.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtjdcnim.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gnstiahxk.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gzfliawhy.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gokjtjodl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszffrwmx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnedlqar.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcbiupnt.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gdpdkjfbr.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzqwdpdqd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gofajqhqr.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ginwohiuq.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glddnikfj.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhfyljg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqzdxpi.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoykwqpl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guqssnwix.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzpqjbrjf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqquhlvjp.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gekfxahed.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycyfbqhm.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrrfbndd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gibkyjpus.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/glmfpptce.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjoqudcp.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guagyzxma.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpguasdib.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxovyzb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfysitie.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbjkssllq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxhqjlfg.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvkenrdv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbhurfqms.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilnnxvdx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkvhjpoox.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfjgngzo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqymhfnwm.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdtveyzi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvljwrdzh.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/geucidqoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfajhnjeq.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmhbjjax.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgqnybln.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxvxqzvg.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/guxkpuvif.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnucnocf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwnxwylo.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbtsxzjog.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzpalwmd.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gtcvpifux.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcidiater.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxpzrogvf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmlwlgek.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoeozenh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktkgcuoj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gnjwqvllp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxigahos.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkycwmrrt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gunwvtczo.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gajjlchpj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/geovileqn.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gshfbuich.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwoqmgmo.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsifsuwvs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevzcxrfu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gturficng.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjvndymd.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmymixmau.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoedtrxb.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gdgxvkkbs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuefpwp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gugwlaxyl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcfpyxkf.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/giaqrcrdp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmefwmeca.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gypummigy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gxgnnimmu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaidezmrp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gjalkuile.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmwczryk.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gokimfraz.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrqspdpx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnmbkpv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxieagbza.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjpkwonsg.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmwjbcbco.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdpsxmqsv.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gblmkkzna.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfhasucot.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyvvyirb.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghielcwsa.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/guxthbwjb.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnajxouwm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfedysyze.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gequfovky.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxikgvgx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gccyyvvby.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gqrehefdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ghhpsfbea.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggjcgewpc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gphirflvn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmlgorq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtskkfski.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/grlsagztj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gxviicgba.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvkvjxwdg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gykrgothr.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gunpzyeqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gboiavbiy.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktpvxzrp.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqequmfij.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/glamiesnz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyffoqwn.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gausibnbu.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvhtxgoy.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghraawbwb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrcteedx.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gziosabqs.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfjpdyol.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzumdfu.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbobablz.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjvnzczqd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gppjvutll.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/grjuaslqn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/grhtvndxj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gkuuluqdm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/geblrppie.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqauzvij.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpztvher.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goepubgnf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gxjuqvhvw.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gszkfmtlt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/grtfqazqo.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnjrevsy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfikexgph.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlcxmntq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gqmybwojt.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnakkzkjy.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmucjyds.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkawvon.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjjsjuo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsuqbiiw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gccqfpmbk.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gdbdcqrup.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjktaylpk.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcmjzbiip.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtjtkffo.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcmuwmng.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gidgwatae.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gphklpbkz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqkvnuns.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/geajjxxzp.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gybaxasaa.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpsnckn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/girtwcyog.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtkufhecy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gldmfuxfn.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/girqxsrhg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcloxmxl.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjfycdai.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gevvyjipd.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfudrzvg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeraotxo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzarsuth.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gggmkczqh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbzolxxr.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxsvrqii.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjlaxvcrl.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gzlluoorx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gowoyzxij.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grqupdufq.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkyolerh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpwmfpqy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzfveycw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwrokrnw.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gklyfdrfh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxlkdtyq.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/grixipaxg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrsvvbov.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzkcmluct.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggfxfpjky.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gsibivken.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtovckqk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhorrltt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/golqxhhvs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkeeqzfi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtemrjuoz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gtvpwcepl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gpbhgodgf.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gxkccehav.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksdqspoj.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnjqqyvbl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gtdumuvzt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gblrvksxo.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfruejdu.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvapdtxpu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glvgpldjk.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gmifoydhc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvyotip.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoxwozkp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggevwflxm.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnvzktcwe.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ghhsdmjxz.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkjuytyrg.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzyhmwea.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmkqoeziv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gobtpkdyr.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdmbeprb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gzlbtaqza.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylkdduqv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxgkakjv.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/geyuogcet.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgmsllxj.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gigadlviv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmibuxff.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiqbeykn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvebcbaxh.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gonwtqsqf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrebznwx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gezcmzfqd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgxuenjy.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdifucfcl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giplpemqr.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gxurpwbox.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubuloazw.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfspgiwbi.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpufxqmy.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gklzeqskv.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/galanbtuu.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcbiubavy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnabzjdem.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gvtnwlpyw.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnpoimml.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/genznzvpq.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gojgzeatf.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghdeqlfyt.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgizles.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbazvkflq.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfjudlvn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gqeycsoyx.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtkseots.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gtruxxexb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gohypfzyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrvpycwn.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grifamqhj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gttotbrhj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqsyoudr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxgpxkw.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdljqyse.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnzvegtb.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchrscvll.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilsarrrk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/grmseelca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/grecbaqrz.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmooqgrw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugazywbu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxmazcaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggochdsky.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdfwyftt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqgiwabc.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/goutnqtvk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/grypogtkk.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/guaunbstl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdxygksi.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkzagshn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gotktwvkt.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnozdun.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdkckommh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gqyuowodu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggardmcqb.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gorvublfd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfapsfmoj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwkaxkpe.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhpzkuey.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxnxwlia.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gdruuvzdi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsewovtsl.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnqnyriou.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/glqolitxi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ggcxpvkvi.sHtML


<!-- 参考信息 -->