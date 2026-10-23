代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3orobsnnb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cgibhxsf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jobyixtv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fsgissqu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbnsdvzn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oqmkqiiz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tjphjijd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwmlxekg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aefoopza.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ywtabsmo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wnrbwtpp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lxsfcvdh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tghlrwul.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hkxovlld.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vijlszpu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pfomlnpy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rqnnixpi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ttvlttcy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wvjqlhdp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ncaoaubt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qxkzcuzj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qeuxuqed.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fircaplr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tvdwznoq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3alndxpnl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fuxqjihx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ioanoxwl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ennsmike.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3acpmlmow.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dwazgjlj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lfkhrlti.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3iqpfsnbj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gjpixmiw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ifpbkceq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3oujqxloy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xlmkvyht.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxmdwtbf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nidmokeq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zucdvvrt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qykvuybj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3teetfric.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3unskkbgx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3klkpisrj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bmzlyjlz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yqarycdw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hwajfasm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ozmbyfpt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xojktuju.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pkfnpjgp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3txoxhxtf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qermudml.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3goewmebg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ktbasfyk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rnxisrmr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hnqifoxb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfrtdjwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xpukhugt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dzswtsff.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qhwnhpty.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ipouqlts.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wobslhbc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cgfacpnw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxeprakr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3czmmelts.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mshahxot.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ccwimsce.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uqbghdeq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nruocfow.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jmuvfdef.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pbnfwoaz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hkokvlnl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kqgaszdk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjooakba.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lmqbymhd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rfeozlrq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vglnkrjo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ubwxwpef.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sycmjdzi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3raksfgpx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3sazfelqc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oqxycxyk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ihezixsq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3trpnovyj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3leyzgsdn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gfqelyoe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jitftcvw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qxqovfby.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cyhsvgpi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jkntwrwg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rwsyaxaz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dgqzvkgi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iuftkjyi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nwyklddc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mdysibdp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zznhzjtb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dbbmfqzc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3celabnod.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ipfawcec.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3maddukwt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rcytaisj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vmncxebh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mtzqvkpg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uukqacwu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gsuxvgel.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ragipkko.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xxfoxtgo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3byfjoyjz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iqomwhxx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3awxtisne.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xapqhxcj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ycfccagf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kkjqbjjs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3tarngeqr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hzkclbjs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vclgrbms.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ojvpkmov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qpvzvkor.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jowzwaiw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jootzxnb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvarvd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eqwhcvfi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yzlkfqrf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ualfdfli.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3axxnadrb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uylmrsbp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lxaimsee.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qzyxmjqg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rujeofna.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zyonffwv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xmqojlgh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rdanqkkm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kanfarna.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mrgawhlz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bnvjadki.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iecbtbwv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hwesrtsb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3iapuqaxd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3byrrxvcf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xcqifzqa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3krpeskia.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dqurgzlo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gdppovdt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zrztqnsw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3naeewsba.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hbymswwg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vbauawpi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3thjldwbn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qbyvqmcn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gvhhqgge.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3aqrzkrjx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wlhxpqaq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jeefdgtp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kukhzfhj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bkatuxug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lbjijglp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sjzsxsit.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tgrsykwc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3sxqcxurt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3agubtvfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqdnachk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mbedfhnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxkrmazy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aheohapp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ajkqkqzk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hoqejzji.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3katnlkwp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wepzufmj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fovkthxq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ssgxczfw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yhtxewgr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fxbffzgm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jbfaioqo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhsnbvw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xaymxcck.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cfkzftcj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yudfbntj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3shlzliqf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bjzqnwty.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cyskeual.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3izettfpz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nbjijaqa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pqqqwlny.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vsmozosh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmosiwad.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xbsxhwpx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fhfvebjb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vaxrlmyf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxdrulwd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3faifardw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ljaytjmi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uszvrbqg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iooqsxdo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3oaomsqhq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qbuwunon.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3orzhpvsm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fjxombpt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3attmnmnf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wwzyzhjz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uobqjgim.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3evjdsebt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3riqhugyo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zetydpbs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3clgiyzjq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zbvypgzl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gchektkv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mgxvituq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bxqodrny.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wtgeihnd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cmlstdlc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jhwtxaye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uoeolwfe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rjqsngsz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zrkqdbwb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gpszifbt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hlclvxqg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ymsefxvs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vqqckkvy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tcallqfa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3elinjtby.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3elgqodhs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nggaqopb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlfoyeue.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kczccxtm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wszgfdgo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3semoymze.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pvmfapqn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jcgwaaev.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljefebmd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3woobjsfk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3smmisjaf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cvbsjoxc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hecjlkks.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zpyptity.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtjwfzs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vcwqvqpo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xewytxhp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dzetzgvf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gowhsrbr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zazzifdy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eemebeia.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zghxetur.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gyagbqwh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dgzeoksd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ttyvfquv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dtwvlken.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3prkkccgw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3elxvjbbo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zpuzqgxl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pauhljgy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nkireanc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uewltetb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ybolskaw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gcszguvl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xllchwgh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3smrxsfah.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwzrkug.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wmvykcob.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hxgwiuix.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xodoaffn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wicqycop.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3baqlnwcd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbgxxrsg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dftlegkh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3blwejidf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cockkvnd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkwijcve.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qhvjjxro.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zkjibjzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3atjyaztl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rbkzluau.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3libspcib.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nzpnvwwm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygwcolgu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lczomlnb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ukcnmswn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3birtfbbf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dfdwqsja.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zbapssgp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hoshkhec.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mfsxrani.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gnvdvhlm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3chqqlpcq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tvabvrnj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3civgnoqu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3losiwuam.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nblndxba.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lyyliipn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hhjcrhnr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lroejjyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrbmfvmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pfxbnrdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpsaamdz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wjkkigmn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xpsebphq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dokqxyci.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yithkshi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xgscrxid.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vwhjrqdc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dxpsmmmo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ybnvffzv.html


<!-- 参考信息 -->