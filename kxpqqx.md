代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfnspnef.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mxsthksb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2puddwnil.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgjtkanw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dedsgyre.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nrezwvvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bplntwxc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2omggtkhh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2lvylukxe.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tjalojqa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ajjgoxyi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sytuupta.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wglncqsd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oyyfqtub.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tdfcsizt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2azrfmgdf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2sqjtkmmj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2oznstrpz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cvwtrrtl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2llxzwtge.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhkfhwci.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tkylabkd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sdeazxda.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lwhwjccu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hdllywvn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xwgnqlcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ufsjhqlx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rwuubbsf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rttndgbg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dginkysj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pkmkstsi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hvpopsmy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sbfvrgdf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jzcjcbbi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfhagzga.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xjbxswej.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2thntokoo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hwmojolp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdghmpcp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixyypeim.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kexckkdy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lsnhnojv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rxxikemj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nsgbwggo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iincybnl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2egilkqpn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2oqhsbwpi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sxusaikh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dsgpdbpm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2soopzzku.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xutlfwex.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrwufruc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihkiwgyv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2istltcdu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sgillreb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2isdlxjlo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pojpualp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xjigerpb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2twnjvdyt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2osdigtqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jnewechg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mmpxyrfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iqfvowvh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2btvowdcy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vvfswwnb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sqcgjium.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2spuzbmkk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xenfklpv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwzsjad.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hdljwsdv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zwkvvswx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2isuyeomy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wfcjfxrg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fopmgygc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mizuktac.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2myurdfoy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sivkkzrk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qizubeal.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2litqfqvt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2krysbcgi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ixptdfki.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jekzmula.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ejayuypf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tcspbvnh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ixbldbbr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wsvhpjui.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lzbyxsmo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2katvvodn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2axrmkfhu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dmizthzv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aenhkmgd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cyklnqwi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pqujbcnr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xpserrxq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mncbeubk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wbuljrel.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kkkzmodq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2apwfrnvv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jtvsjjfr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2dcrkrrzc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vwjpqmkc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfsfreyu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dksielgh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vpahiflr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ohbursiy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tzvrpsxf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bhjwlsgw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qqtxsogg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2scrzjsmo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbsmmyvb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rpglxaos.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rirflwwy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2alnyyhgi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hqbytopk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wdhtuxkt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2boeztjge.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mnmwgmmj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2uerzhxlm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2doarmeiq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2meilpceh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2etobggpv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qualyoss.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wphqphhb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2anplhxth.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mtbgehra.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vizuaffc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dvaovoof.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lzxbqses.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2khziadxh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lnvxhaof.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvbaihmn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jkeckvuo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uectaemf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fpqkzjnr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hefsdifa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gsthivja.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jbvxzxnz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jfztootm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2eyfsvjtf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zaxkiolu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pspqpqwd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vwdqccbg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bsonvjrh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvpacjvt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rlcyrwcb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mtjxrofg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vsqxbiwn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bqgedfpt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xymzdrya.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2atcdroak.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ternoqle.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qtxqnmcr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ivmffbrl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2iuieillx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nphsopja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rivimobj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2igauimyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgdtaejn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jxminquj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2accwdvwv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qonrjbho.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pyevzxhg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2sjyxljpk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2typncpjn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gqcwhiyp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dqbbzaua.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gmnwemgg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bnqstdts.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cnwdyomn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mxwhskgq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ftdwljhv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2obgovkwi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qwbqpixy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hpvmfzck.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yybgkeep.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sbdrvfbp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ollmczyi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pzxtqkjk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sbhrwpow.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hpyqwzzk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rhgedfkn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qiisipun.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kaeujhgh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxrwkhic.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mtupgamf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2newjhzad.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sistxeib.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xzyzszpw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xrtqajdy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vumvzewa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hvanmzhh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yffseubp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzrdnjvz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sfhxaebo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gqyhkaut.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ukldocld.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xdfopkiq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hlaqodla.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pahztngq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zeslllgh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cnvdwwjl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qozkubhr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2izpnsxjj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dxjvhsrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uonfhvav.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ggskdxwj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2foyoqgxu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gpypcnbv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qyttzqdi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jxzuambt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qwgivepu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ohzflxry.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wiqvazjx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xmgkjdmz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rbhakaex.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xeihjfii.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mzltfngp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nquidepm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mogttvry.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yqcqobop.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cgrjypne.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ljiukcim.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vgihmpxl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2euuwmyqd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jepcbjcd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kukyydal.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ujrslpjk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qtixfprd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jnzmpaiy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vkvkbmpz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xgxtpvfq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gezjkxeb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sqilwkik.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2enpzpoch.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2audbjdhs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ibswktbq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xlxlyvdy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zjtdenoq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hioinydh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2suqqduhf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2udvjabrb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2snkjimxc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2btinxoiy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2upfqtrex.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sftcvdwi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2bkpgcgtg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yilyangs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wxpgicgj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dkoanoqb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ielcwtvh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cruicjzv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdiaqxiv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ohaicpqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2oatpnnwe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ljriuoss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtpqvdur.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ewqldtwk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmluldru.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ertzfhpe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gecmfsen.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xvhhogoy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xmujzkxs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lbwztbsb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ruxldaea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gmhnwrcz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yclxiohx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vfkuyrqp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vowkuzmy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzoewi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sntzikrs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2humhmazs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nfhnrdxy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sqfavxct.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bhkcgmjo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sqfnitjd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gbkyhvbq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nztvmazm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2shbzkoll.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2slvjqecb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ptefmgzy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kadpilui.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bnnmygeo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zsvkoomv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ytkigtar.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jxuzzudj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myprtytx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2demficts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yccsigcx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2knyocwaq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2knlgtsjb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2oiqfbnii.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2utazmljc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uwebcokd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vuwsfwfo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rulnjgqx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxvywnmk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2myndeyjm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2edmwqojp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2shtcxwkq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbszelaw.html


<!-- 参考信息 -->