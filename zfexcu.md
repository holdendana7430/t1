代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezfvdzfr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3oecsjkmf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyuszdlv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxptbopw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fhmjtmhq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qchlthah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3khqcnmmv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kyevzfke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tvldanem.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wprehmth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lasynama.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3schsfbhp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3lrqotqxu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zgyfrqjz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3uecrcywm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xvtpqqba.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gynnlolg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3psavkzny.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vfwofrfv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3boyuxifr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3erazkgcj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xdiarhsg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pkdfclgm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bzyvvhtk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pehdthfy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fdkbrfxr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zpuugigx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qajbtiad.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqabtgpm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cmdkonrx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfygmuec.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xjkmafqz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3aaynagqo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cxgzrsqn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cdjpgtdj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bgtebxrw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nnqaczan.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jexnokvu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nuxhsaeo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qxgboffz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3oajcoify.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdrlflmc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivrjxwis.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ttewvhgu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mirvzvhw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tgnbyrsn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dugcytzi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3amworcab.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tqxjpiob.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3djmoqkba.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nxsmvmtk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3djakyles.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aqpjniwk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bvntczfa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3szltyvne.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3czemwduq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fqciozha.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bifgxfdl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3frtrmiic.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hbndmxhn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fycamiyp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jgurzsbh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nezredsz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qhftqgsr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zmcqmgvw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3opgaekno.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jjexfspc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcpikjso.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3suckqafw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ctfvibmy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jonwddtq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tycwiymi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qzxbtpid.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bnmwrstb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3erwksuku.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oyythjwd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kyrizsha.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ianpiahk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tiyabiuv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dooyjmmx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oigbowdt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qqbcxbbm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fsxpgyjd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aiipkgej.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ohxarpmy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3btctadet.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kicakpch.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xkwqprsi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pzautgte.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dedeewap.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gsyyjmdl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nxebgrqt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xuozlnyf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uwvkehwh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ycjvqnmb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3oagmmabp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3countupe.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ileddhuy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oqmdtgoo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ylzulbja.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3plejocdy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcikpvha.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iseqjppf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3szhkysma.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3elstusei.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qfezxrew.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tivdyjmk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tqzlazcp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mvkvjwog.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3smomapww.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vwrvflje.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hhfetvxd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lpxmclyn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jgcvqtso.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jqcrcngl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ohlwogrw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xzriiuwo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3evpuysnb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hssxurjq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ckayavdg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3axahpoqj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3juiwsbhx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3prujbcrd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3iuuhlcdp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hxjudmss.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3moaheaav.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xchpnkxx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wklooxdz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mrdxueaz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zecfreof.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3scqholzs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3aphoeqwd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lkjegcsj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tifbhans.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uijfxcyg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3daltqtrp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gogzmkur.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xueobqhp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fgmcdgdc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gbgshbzh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sksynxdh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gkmfsfzu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rbsomzsk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wenxoqqa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jrqwfhec.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pekrlrjj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nqmxnvgc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3piokyprh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wusmsogs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fnpqjbrs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bzwddrgf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fkijxedc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ncaferue.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fhymkrjs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lbvlglak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcycyrbk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xijahdxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gplyhtqv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rnqoepiw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lcgbqyyf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3joaekdrh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sxmabelh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3japjtfeo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3oldmbbtd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lwdbshdn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sjhzsthh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qoswfgfd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pcczlbvg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3imuvxqkl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vdzukgwe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kkvkfocr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qkltrzkq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yhrrvdkv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sibvtjrg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3blehewmw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3aztmywvg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hcwgbhbw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dltnjsrt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3okloykpe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rljubrjd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nrigczbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oolihmji.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3atuwtvgs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kuxsrpoa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3elnlaeti.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bdxrlsbk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jfaowqqb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xwoxkwhq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nadtwpfk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3huicthsu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mqzdomly.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zvrtvogt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wffbjqqh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wtmtzfqn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dxtrsehi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ryeiwkko.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mkrwlwol.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zssimvkm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nsvfqzje.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vrwgfpey.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mzzjhflh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3aawivfon.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xparzejy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3njqzbfvs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3afkzbqdp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yjqlzmxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yxiuhmnq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hmswjuno.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhhvtog.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tbgkjiil.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wudqkdfk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3thwxwgat.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ovktsjmi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dkegupbc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tuomryyn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dpuemcww.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wxftelqn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hzlwkeci.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ydtrhapy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hzexfcky.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pfceqorb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cehlkskm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lggjtxzk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dgueomgn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qtshrjvh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cerbhfsi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xguxdnnz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nverofsi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xazogclw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wbjzuahs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yxbdltfy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ugxrtagv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jjtbkgxm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ywqorssp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mzircvsu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sryiwizi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fcyrqpfq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lueosyvk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dqweiurx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xhluuwby.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3soxzambm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bbapgcsy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lcvgolba.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xniefgna.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3trtlmmzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pualezyf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnuxkkbu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fagqyzog.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hxjderlf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gglegopp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bggiauiu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tozvmzfn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3smdnazmr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oackmbzb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3anxvkggd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycbfkixo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vobwrhip.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pyxshpth.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iodfyqwa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qqozyqoi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlppewb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oudqwhoe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3movpuvzn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gmzbblhe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xprszyqp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ulqldodv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wdzooezp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jhbwsssm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hxzifhzo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3okagpauj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ckhmrpbd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3sanrpefs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vkfyczqu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fijalfjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3emtctink.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bhfknxng.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pmoamnqk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3snrrqnmy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3swkbpuxj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fcyovcky.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3musqxumt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wkatlnse.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vqvtxixw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tbmcqcem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tsnczsps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3loiuyrqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3leavgdbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baqujcmv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bofbotas.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qnwjajdu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfhwtimo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gbyprkqw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3biortlvb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3usffptto.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vnjcgpts.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vesyzzfy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hkglmadx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cshhtatt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uowhlooc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dvtojfuj.html


<!-- 参考信息 -->