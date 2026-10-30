代发 wailian999

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwcmehad.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghrgdrcle.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gugvopafu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqillauh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojwsetus.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzohvnqb.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gzwdqkfsh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwuuipyp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrzocsjt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gqfpeuxxb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkvwerpmk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoeilufd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geunjrujh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gomqoppie.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gimilbzbr.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghjjgubac.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gvscyqyob.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gvlyfnqto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gejutafke.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gejezlvyx.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdozjsxm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoimqfzq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgljkdxy.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/glmpwssay.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzjbjyqn.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejknsqae.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxrbhablg.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyeucxsi.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudkuidek.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnqepwx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrlutydv.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gvxaovndu.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmgnsus.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gsondvoqo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdweofntm.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdueulyac.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/guxpexdzi.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gykxjsxcj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyujrrxnz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgyobjrt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxzkzzuyy.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gnxhqtzgz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/giufqabfg.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/ghhxhkcsa.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/goctdmjdd.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gicfpfcgt.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guehdgknc.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmqvneng.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gtntpszrs.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghnrknklr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gndfffhjq.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghuztptwe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyxrhpask.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjhckqmg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqvhozyk.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gakbushmj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqmldzqom.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcptohkzz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqczihcvm.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gntundvob.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiiotzcs.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gacmscoko.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggklmzcvf.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/glqafadae.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqalnpghn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/groyzgmph.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsassbly.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxfvsktvn.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjobfehyc.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtqrlms.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkyizoexm.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrvwygd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdttufds.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grrkflzfp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdavphos.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gfldlpalt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqehhqeip.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfnbxmbf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/giiscmkje.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnrgkngb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhzblgiw.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gymccwnvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvgtivte.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpejhakr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfzivkzrn.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gmupmxbsx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/glxoxxdwz.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmllueulq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpyzbbmv.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gvvehxnlp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyakzxaed.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhchtgor.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gisqulryx.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gatujvvfh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfjkdkkg.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpadvphm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubachyuo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyijmtcwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gpcwmxyzp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqqljjln.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwbpqmdkm.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gminhrkml.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooobekxt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeccthxn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggjjfqyzy.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/grqtzeygs.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gscedanbp.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gawrvcdid.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/godcqisow.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbczgwqi.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gocgynrva.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gytmnhntp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdciclse.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/ggjagyrse.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmqsneqh.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gakjwgqtq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxptjedup.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzlpkzch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcofftsvo.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcdhlyzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqvgtasfd.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdxulbwpe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbqghhqs.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiswssbh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gaglvfljr.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcgmbxos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsoczixok.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gefylpfyp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrpbtyxc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gwfhdgant.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyrjwvwvr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpiileqj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggshbnjay.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsixhamz.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmgeqverf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmvhvcql.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gcggyaifi.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/goqdmpvvf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/grkfhccvf.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gijuehdko.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gruuiahxw.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcgbkezh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gokrktiwt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwglxggif.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gykvrttvu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghumymvma.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnrslsdxq.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmrbfbrei.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/grmsrjeqd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqfcklln.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gzsyiolag.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gpxgpuovp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gskzvpfzv.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gootteqgh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjnrsgk.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gancghdhm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gknyjvvdk.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuaykxmj.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/goowycuun.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gltwbjzwu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypsiavpx.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlftuteq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrulbcgm.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzznmjhu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrsjqfp.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggenzclpg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvrraqlo.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpemehznz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddxjjzyf.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvmscgxze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnguydrgn.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvjeszlg.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gwvabfflu.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/givrlthko.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbofaqfpn.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghchogwds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gymrlmgxm.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwhtolvli.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gugczsbby.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gdziyridm.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gdxgpqwjl.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfncakzg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxytzliqi.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gobpogedz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnokwjjlm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdmvksiv.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstzdemsi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupaddrq.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gmbhyhjkz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbijhyhm.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvxmfvex.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gluornfdt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gogqsicyf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/geuvqwbek.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkfbfbpd.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gnarmlmrf.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/glshhjdih.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqpbtjmo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gycezpwkb.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/grmzztwdk.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtudnufcf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gairtkqlp.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gtkjemhdo.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gawgrxfgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvipmfdnr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcltntaw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gvrjrtuoa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdescyh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gziseeepa.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/ghwktztff.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcijgxkn.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grszhonco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gpdmegucn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gloabvyzy.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gutjwnahx.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gifugngtm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktkvyoa.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlegdvzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmirzlizl.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkzrkmng.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhxihtgr.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gczikwqai.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmlsljmr.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlnhnrft.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxecqaluq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gdxqkdxzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gvpmodxho.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaninwvs.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gacshxzsi.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/glxotucsb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnozaaza.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gjoqjqelf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gunmflvmo.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gksruqmdg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfbjkpdt.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/giimgdceq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxsguufsu.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkxkyyxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gilvlxbxn.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gyztsfyou.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/grgxvnijz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffvyltlj.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gslwhmopn.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwkkfknh.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyffwpyvp.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfdhtocfd.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grorjbwlh.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/glqdrscwd.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/glgwdlhqp.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjptpera.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxmkhcv.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuwpcvn.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gdkfagryp.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gqwuwlelb.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/geelbmgmn.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzsuxoutf.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfwihtle.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaseedykx.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjekvojyu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuhsueik.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowtzbmua.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gaqhevqvz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gthcrhcyn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosedisnd.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gclzuaacp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gluublref.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/grutvpoju.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gztvrqufm.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbrtdqkc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvxpebldl.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvuczfql.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxjsaitm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjajoluba.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqmafbqr.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdnarxzf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbbuqiii.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbigfmmtm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/golcozxee.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmccahfsk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmwvfsug.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsjhpgar.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gggmmwvhv.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gmhssysoz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtxkvjug.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclaaraeq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcxlzaoxm.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gnspjezhz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvyeqdjo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/glkehwems.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbpyscre.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/giyfxclav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gicrtkdiz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaovaygly.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcfovymik.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnagoewkp.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gfeuqdhew.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyimppqne.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmhplav.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacntqsl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuoyvcvv.sHtML


<!-- 参考信息 -->