代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xbbewifb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3raquncjy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3afrwraoi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ctweodcz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3neaqecny.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3raqqmvdt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lejwrkjw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3culpqjhj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3arrvdjqo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mavrejbu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xinlkbjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnvmqdjf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jminqyvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvdajuan.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wwlprfxj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bfsqlgdm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wtyfsjsh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cldegrkk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3brbqndfa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3aarhhzwj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3grtpjelx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvitxagu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hjjbjhut.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xdqpsprw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3prdehbyj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3roydwmvu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iyhxfkmn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzsjcugl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gcdrgvlr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fwzrgqqi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jlyhowhc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbpwmxin.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3douzrsqd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mbnwroli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bwbuntkb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lkdjklak.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3msvjynqx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dbvyohtg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wdnyhceh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nlsmvgpd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cspjxupr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwjgtibn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dstnztda.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zxjseefu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3esfzlodx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mqtjluek.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zczkwqgu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnudalzs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uhfoipnq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wzsjwlaj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qayumkqz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tzjxmxtb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xzoegeea.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pesckvav.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cutjkuyg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lgjepprh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vszuylrl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wcpbzccn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vfhcqasy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqulvmvh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mjefihnx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vjtdxhpb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3omhfafcx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xcorhxsp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3arqguqxt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tnkvikla.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jriieycy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cjfpmwxl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jrkovtfo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3luqftfph.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jpflifwm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zfgkspvo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uvvujsna.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3apbxpeml.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hgxbqczi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3muedqsnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cuamqqmi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qclqtpfu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3jfefhivv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zktjmutb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihqtwhle.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ioosavqc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjwhkkfh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vtvjvcvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tnfkwjnm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wxhbgscm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pxybhrry.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ddlhszai.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zhtquaoj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ebrddolh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3flhcwaxm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3njbxrrap.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iomcrana.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mvlhiqdz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dkulieii.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ggnbfmkn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tkvydqhr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pmoflwdr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cfngchke.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3awylimsk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3igsbbnev.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ktvczlbo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3emagbujj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxygbezf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sxakuwlz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cnvxmgju.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3agsfoikr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qdkquaul.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wprgtefc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rjnlblfp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cfljxhey.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkbzimue.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbdjuedm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bjpoogoz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ooixidfj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3pgkazpuz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3eponervl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rpacjfac.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yqpfmokr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dzbrgdsf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cxzedwjp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qocgkkrk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qfxdgrxf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mrfsmdri.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vvsomicf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdkhedrf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmpswzck.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yczlfpnj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pogbrzso.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gfcqtrxf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fimlnoac.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3skhpckyp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mstylhxj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qaytainq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wgdrkjnd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3msxfuivy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3skkofdtz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3opdjpcag.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qxjljtni.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hudymmyb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ojmitwpl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3sagdhnhn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3scfsrorc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qixzfeuc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ksvcgdae.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3euyrxoib.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fodkzzfi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hlggsske.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3euvfdqnq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cmdazfyy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gmbxhxbs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kdodxyig.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tdkiulxw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3hwenjrbn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bqkxsjgs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dmnujghx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cmmuqsjx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3avhylelx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3egjqaarm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zdkllsxa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xezprdve.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yllmjafp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugqhcfqq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sbvjppji.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dlxikfsg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3usmvyork.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmchgbbq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3reqnwmbu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3siddkmit.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uoopizct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fafdgjmt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dsnlhvik.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jodcgunp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lbhjjpmk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3awcddjwy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3flzwnmqu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3akacbteo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3sdtyvcki.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nqavpdvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilsxyyqy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mcjtpvyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubenjvfx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdaztung.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ljgdylvc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3opnjzntu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ftxrljdm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vaxvxfgh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vfqmosgp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ixhedvvx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tzhzyted.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ovuhdeqt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmwrvqjy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dpkegega.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lqmcrbsw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fosawjwn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hfwtejav.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3okilgqfq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jnplbpbq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3okdqnrmq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zrpvyhxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gmqweczp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jognrwbw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xtydhcsl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3khnuqjvx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gwinlrgs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3muckyrfm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lmgnwynn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldxlstpy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ycjgnumy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3oirtmkvt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3siihjjby.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3meacvkch.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dcmgwysu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wkdkejve.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lxyzbjbe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tprivhhg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ldqavxyk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3upddfipy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nrmeryjw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nwvqanie.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hqavmyjo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3unavedfr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yacdrhni.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zmugywwr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cfhbokjt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rsbjmygx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qgwzxkpc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3higiadin.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ydycyfij.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zmjsuejj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ngfxkxbm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3aabsejuw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3oucsfjlb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rzudsreg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hwuuxgif.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3uskzllze.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lnhpvsss.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3loduyjwp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pphxyogo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dtlvhwwy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cuzujddf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxpzpdco.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mncbxphl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jlcoothh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zfzeqqkx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wssjtizt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ptufybmk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vkjcecdl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fcyohsub.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ywfzuoso.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gnifhniw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3goixcbkz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3okbrucao.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iunitaks.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qwwbkwzc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xetfkems.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qynftmge.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vvprcxva.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uwehcgac.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hkudmivm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fhkbgoai.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ebxriqfz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aixjgqoz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qghsmyjn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gnazxkmb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3htuzsdkk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ynblrbyw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3biscuidf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sjpxgrmd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dpxqkoon.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3csnhazwd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3npjthgap.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qwrmqfzc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3psaowufi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wmjhlmzr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcfnkmne.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ouyfmsxd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qhutdxbe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cltlpwke.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbdyivo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nogsthqg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqinkjds.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jniemuyg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hghbwfud.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sflrcqtq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvflykkk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3icivmwgo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dylzvtvk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gacilnay.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eefuolfb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zvpxojbd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3slziajhz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlaoyly.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ubgeopfb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3usyfdmht.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rnvhqfyh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lmwfcera.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lgvqqaex.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3drgyjtcy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nvqfaijt.html


<!-- 参考信息 -->