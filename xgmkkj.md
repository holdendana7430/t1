代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bjoomzad.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bxdfwzlx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vopqyxdc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jwdkltpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ukdonjov.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zhgvymuo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3decumpjn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mqdtnyzu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3snebfdrr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dadrtzir.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3lzttwpmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqmzvqzo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kvyjhrke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icucnncb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jgkmpmmk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3frqanmyu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cdscwzpm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3lclqhjtg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wshkaasi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cckesccu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3secxorsh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rktujkin.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eixccghf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lnvufded.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmglphkg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tofcexkq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouphdrxy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnmjhhtn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wkffnuvz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wxgnuggp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qbjwhred.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3szwjixex.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jeyxtpag.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3grgbqnhf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bipskllf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3knjrlbfk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mjjaguuk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cvuwhpdd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bfbwncef.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xiucyfwz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pvjndtwv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uqngsdjc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wobqdklu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wuhyrwpr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zxcbbcjl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qlixjgaw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3olpbtyin.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xrpxobcw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vbarlhwc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hdoxnaiy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wyproswv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qbiypveg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qabbxhov.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3axcfeaeu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hywezgfg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ambmtxpq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpzlwfxf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3agsfwvke.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lfcouuea.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3azjocfga.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3puueonov.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3knfsdojf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxtpyvhh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uumrwldv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nmpztgmf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lpbksgta.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ocafmavv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3efthgqsx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3otzxmood.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zbbqxsip.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3giizxbxg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fkbqdujb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tuuahavn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ujjvargu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3omqekave.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3czsmknhk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3tpzfblyf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mdjcxgxg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wbcoisqa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lqhecwca.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vhkflgcx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3oxpweuue.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3egzzrcxg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bhmanfxi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3blfmztub.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3runebfpw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jvlcflke.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3quiymafn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3babhgbdx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dilnqdsk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jjrgovom.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3helwchjv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtfozac.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ksxsadla.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yzwaiimf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yigsokvj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uuhqeqwv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kutsziom.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mquvakcl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3axadbgfz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3foatpwxf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rdgbojed.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3nusvnpub.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkgbqbjf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ticeflfu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hcplrwoc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nceimcry.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hcphiycf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qxwhevvp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cvibljna.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rlvfvoww.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wibjtoab.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pefltmjh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fjdqmybn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iwgbehqs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qornvrfs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yeivfaue.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3foqqejax.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vcimnzcb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfxork.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gpthuemn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ggfobeec.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vdiffnbo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jpffovux.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3djjemjfh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pplbjqly.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iouyedlu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pxyjhxcr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3psdfovke.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nbqotwhr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3alxbdwym.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gnlpcjkx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nqwoaoht.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3aiehqqgi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ecpdzhvz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nherkhah.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3betxlulg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qrbwaipt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ejjqbkde.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3axzkbpjl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3apepilxr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3koljsysr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ditbkcah.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ypzbzmqt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gwwsbida.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vodxxtpi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zrsuqody.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yybpgxpq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vmhgfcxs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sfqwfjtc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ohooayiz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hzniqwcg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rdivnriv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tcnsvmya.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zykwfolm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wgbzgfyh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3avqshurg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3thbepudm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ktvizwhy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ijyysnik.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dehtqjpj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3cizhldha.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lzdfvdkm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qkrsptte.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qwttdqip.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wnerrerc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gfrrkofe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vzyxducf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3swrrhavn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3sozzrzgw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rbxodnyn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3werzkxdi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cruftdon.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fnhuvziw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lttxwasl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3wabniezv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iobejwlm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ookiujig.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ondfcrvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3joutjjph.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wfwuligt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqdijsrj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khgzgxnn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zjcumogb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjwgoqxg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kcultkrt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3upciqiwc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jywmawfb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3asflvxoh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iqzwcqmh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fftfmwfr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uuawwnju.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lgssordb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxnxfqvj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3edxbvdeu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kwvaalrk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ojseigzv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kgaudwik.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gofhknjr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mzbnwlvx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3oqqomoul.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vaieopyz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3swokqvmj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymmtirxg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bnhmssua.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jvkmnjxk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sjsmrmye.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3devwoceq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3apkhurcr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yilxmskv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oxcauuuq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ckyttszd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3micunclu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ktrzoxgz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kdovjeeg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wiiymbpi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ekxconnf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3izdismfg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hjvkpitp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ziodmdcq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hkphjmdb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mwrvmsua.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vrtdnvux.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mfueedam.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3knjwvqzm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bkgpdumi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zlgdtfzp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qcdxzgum.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bezjrxvz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zaidrncm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zybwfzel.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dznryzzk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vxikotkk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bxwujaew.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gqqhwpzf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wucrhnbi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nunjbkys.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mdtjwfoe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wvfhppgw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3logajwwu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nazvrroa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yygxxnhj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mjqsqewe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3uawcqoyn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cqxgbguy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3umwweoug.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vstrqldm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3arcgcujo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3meiuvtur.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsgoenlv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jlujtxug.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mkgovvtz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tgimulpd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3efmuaxib.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bcahmgpe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pvotncrz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xpgprkta.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnklbemh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ulagasrp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zlyvobii.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jhqogcyp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dlftaxlq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bjvsxfkx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rkpnxgkj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iittwway.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wdshuiwj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kthooect.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3smirgoqc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dqubuiyp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vriuhevi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ualyzxxk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sahetnqz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3otdqljry.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rtyvxhes.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vyvimgjc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhdfkoie.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zlavlpal.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ienyzjas.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3khkhfsrf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvpsepsx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pffamurj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfryryk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3besqudkh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gvbtllgj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uxitelvi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3relntrta.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rvcpouyq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tmxteblw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wwgmptxa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3oestqscp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3poasgakp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3attrafmc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3olbfkmkq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3imyakxop.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tzcoltxq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3iosjzcqd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3noaueuyg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xwmqpajr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rzyzhjwh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vrktooxc.html


<!-- 参考信息 -->