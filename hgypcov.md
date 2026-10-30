代发 wailian999

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gofirekhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gevtcjalo.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gymhkvhlq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkutazwqr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/guzittqpq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcghcqfkm.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlhtalyw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxemlemya.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gaztbuhtu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gwdntkztj.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjrlvpvw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gkplihuun.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavaunjmo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gdotxlwjp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszwrsump.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjlnjchx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/grbpjlgdf.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gulbgmfvf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gruncqdlp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhskydmn.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gopgwoeyc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfkedytwx.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gcqfohmvp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxcfrjrh.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/goewnctzn.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gpzvxdzew.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmkkdqjh.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfmcagko.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gwklmpype.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ganugddnu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtshsuno.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gqhxfyrxd.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhcewsy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gesrzekkl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gifpufcxq.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gecbtfimb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdtxwdo.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghgbwoviv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihsaauos.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmbjiskg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gczmnxlvv.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbknhcgze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/guxdrynnt.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsbuphtv.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gsezfnklq.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwazxleec.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ggqagahyy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxvgaylln.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwbfemg.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbvsgaed.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczmagsck.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiekitkp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gutclecnc.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcmvlwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcppwyok.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjarjxlp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggwsphqux.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ganirpgai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsdbehgj.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gugkronit.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkurqedey.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghedvqtgu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmboayak.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grhvplxzy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdwslaky.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaqiflnu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpfevpioq.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsoujkyvm.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsnfpkmyi.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gdifvmpkn.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdmqwcqll.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsinrfatz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcfjwpkx.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkrfvdrr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuuqkfxt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxhbbpys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghqkoxpru.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnhtthpz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/grstbbmyh.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gqzgpeaup.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gxfdjzoyw.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gbatlalsy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfyljxul.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqxekzdf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjbbnkpge.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfwkfxli.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gfltlvknq.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghuefscfb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjuggbbvj.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gteslcvcx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdduhzxe.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gubiizklu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqcbhkzd.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/glkzqivzx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gzivdwthq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gauszoobr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdxidsqm.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwbtwfqyp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxunholz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxvtrcyh.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjjrgml.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghniophkh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwofppmdx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/grgksuvjv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdxkhfsyz.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghmnlltdd.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gzgezzxrv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnlmxwdq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpytsxb.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gunqvusqf.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgttjaac.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexzeffor.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfmlxzfk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzsqbpgz.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ggseswrku.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/ghlrbjzez.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gutglbsgj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxnbpzsr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gvoiyrojq.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxrebhzsc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gebfbcbrl.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gesfphqbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/goubmdwiy.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagjtmmct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/grnsjijlo.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbqqqxge.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gomsthjed.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjvjbqnu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gglupfzcc.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbixlss.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrucwnxb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/glfculqpv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdxcagwxy.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxrrrovga.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwceewnn.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/guarqjryu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexjzhky.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gafljaest.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gjygkdemw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsvenbxe.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gkwrdryck.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guyygcrhp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykenqpy.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtrmlzew.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfrverec.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gljijlasl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/garptgtge.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnhxiwwf.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/godfgeikw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gihuitujy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/geeqgnbeh.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/galkldpit.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/glqxinkgy.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvqbcmnb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/glnuugska.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneujxhep.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbatfqjyl.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gsycflvfu.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gyicnroaf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdyrugpv.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnjyxqia.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gejhjoudb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzqoprkrf.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gkubwyhwt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcurngya.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ggfbnzicv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gchtcybbd.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqldghjyj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvswmbkq.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gsexgomzz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaatrbqi.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqawfdoa.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gqwjraubm.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gameahppw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeiwwxvx.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glcizyrsy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtpqjdgq.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/glqbvsutj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwekkjvoa.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/glzkhleoj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gavngjitu.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/guiqnexwo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwomqpvvt.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gtegnjfsl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjndpqh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/geuqahmva.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqphlzju.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gseqngplg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbrhgugf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzognajjy.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxfjwdxj.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gwpdluzwz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjdatlgix.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gikorcfoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvpqcyvw.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gdydbimbi.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnbixyo.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gjybqyais.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/givqtstgr.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnhorgp.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvkfbotc.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggxcnexfm.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gkcyjokob.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsamhuzlt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtxbquck.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/glzcqkqxt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gcotghory.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gorvivynq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/glpprklvr.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/glnnkbpal.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaxuyszn.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqtbckyyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzudonkr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gztfzxhrh.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvodpliqo.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glyimnixj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtnhgybyp.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpslbbma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gcclnsarp.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gjzoyomvc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gqwseipoo.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzpnyhfw.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqfvyprnj.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfydnziap.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjejtdloe.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxpxvpnn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gaxmvuiyf.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/guveohgbo.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckrultfh.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmymbszk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gcirfohmq.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpkzfvi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvbbodhq.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gipizgusf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gtfgbvahf.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdiapcvge.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcvzcjyo.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goobdicmf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfilfgsu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghcihxbjh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqevyacpw.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwnxehpof.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmsieecu.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/guukxjcnf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmwfyri.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/glafxnuoo.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gopfrcgtt.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gomgwvtzo.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/ghabttmjr.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwcrapvx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gwetfbuju.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gvabopqiy.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gyqnchaub.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/grjygwnui.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurukobbq.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmaavlyp.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgpafkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/giucttlac.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gabonkdvl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gywitcmdq.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsgohrlq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdjeexep.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrejwogk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtyfabzxd.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gztjmpxnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsusgkcw.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gubzwnhyq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggapkugfy.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ghoddvqii.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/glckwjtzv.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjzlujf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvqvjyog.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnspehvo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gefcadctj.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/goikorjhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfocswuz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvqdouvr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmpxttbaw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwfifnfbh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnohrdprt.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaouqzkh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmeealgs.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqipywuz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszwvonlm.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gnmrnanot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfluaejw.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzkgusrj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtedjyovk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/giuwtqrma.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthxdvxgc.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gykblbkla.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiwhsxqq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gfciarutm.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdspnqkao.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gjnjnpyxh.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqsszfwzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/goqdtbuft.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbrsgbx.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gzwzccrol.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gbrcjkpgm.sHtML


<!-- 参考信息 -->