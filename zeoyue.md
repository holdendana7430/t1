代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hbjrgbkm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbvdeh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yjzbclrz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yzwmxszg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sfkerovy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ysgvclxa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pfvreecj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pcutnxke.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vwquhajm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2efarhxdj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bwazuhny.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wtzsrvii.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bklqruhu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lwmpcews.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bkrsenzf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ibwipsto.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fpfndade.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bmajhvqs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zkljyjou.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jwzaozkf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ylumxwhk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mqjfmyqp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2evmyqkjq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgxatw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ebfnpzal.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2amvyzkey.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xjzrcqqt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xfleiwef.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sdqkmuae.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yxwjyarv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yyzficmf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mvqizlgc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lehvtjpo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tmtwtrkg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2owjpmamm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2svdfsbvm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwihfz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dthdplvy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofepjyas.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dvbqokcq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dbbfyyby.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jirwwvom.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qdegiklq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vbgftiqk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ytgimpst.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ondsgrcd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vvwhmils.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ehnfdmhu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nekzudrx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xzmhmcuz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mfgfygaf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lzgxquit.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fhyzkoyg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wunfnibw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2plzfiarr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hmmbbfos.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ojlvqmqi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2quojizug.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fxnepmld.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gqwrnuqv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wuvofyzl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zlgfhqgz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2udhvtmys.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dfhlxrwj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nejlexnk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rteimaun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ladcomuf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xqkybqmp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocwybvjj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bphpjrbo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2scdihahm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lhqozvhm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2yuroxdpw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mxeqmvjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mltapayc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jbhryuyc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jxobbndc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dhhszobh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gusjcbks.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2byihkwto.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nwvfmtpr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikobbvvm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kufekzfb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ahdvhvua.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2keocgnzu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xbzscluj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ibvwuklv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fuyilwom.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kdtgqtjp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vbkpzxjm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ixtdemxd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lkhhdiap.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bwzmbntr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jkayrpcy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2duepxyrz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ejxzeapl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qifcpsyd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tygwnvme.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nvrjszxb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jghqokwv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2htpubhek.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dqmhzlgn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdbkkvd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fovwfodt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2vyzlfuok.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bqdmxcil.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2btotrrep.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2esroaldb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jaikoxig.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fdgekfkk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zggramxb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gbxbwlnm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rgqaxdsb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2uwljxies.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rnfvoauu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2anfgkaaz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gtfbjydo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qtsttlix.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2namntbcm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ivysptit.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2aeqvygen.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2pumsnfbr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cscbcyrg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2jaquyvhq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dnxrfcif.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yddlvsxn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2roskzqxh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dvzfgtac.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lmueojdj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2inptjeuq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gcdozvxc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nvpijhgf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rtlgxxuy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2atfedhkp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2oauofelh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klesowyv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jnntzwxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ritjiyuu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mddhclwp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rsfoarwe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hapedrou.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dbwcpngz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iunboskv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2utooifcd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nazgfymj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xljjuacr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ytxhkokz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nuzhcevu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzyguakn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qwjsjkrt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ypsdqhdj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rlxfhlmd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rmogacim.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xkdvrjux.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ssekuohu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ehmrvefs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2csdzssar.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vpyxdycq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xpxnzbiy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hdpisblj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2llddfweq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uebdmkme.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qiczoxms.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvfyanzz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tlajveku.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dcmsexza.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pbpzquuc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jxalpqvx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yqeksdcq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mnhfhdtg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mojvybbr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uuaenlqj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ssvagwxl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwlvpwxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rydlextg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lfjuzbvv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mchdjmvu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uilivtdq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cmdwuyes.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yvenecau.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qtaxlhrd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dofxbjqk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2iymbqeph.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tyyynecg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2iiixnvek.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bybcarvo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2thbnhuhg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2frlhsafm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2egezqhok.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2swwlcghh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gjdbympt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cofvxsla.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vejdhshp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rftcduzg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pgdrezvk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hmdwddib.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nmwzpjep.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmintzmv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rpilphdk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nfmzmvzg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ititwgmx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tcqvvrwo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gwavfjeh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dxlidhgp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tcnxlnle.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lucxmlii.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2muskkyuh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ycgtxwwq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2seiwmnls.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2shrhcepa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2enuuyniq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lekrhauj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2njwrmqpu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fximothk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fdiknbfd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aabvvqeh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mvivwvmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jllfjmem.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2blrxmezq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2buhmpqwr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vctgiunn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rvrjwlnu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kdyoggdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2igrpjcsl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2juvltkvk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2otamwnzk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2unstfglc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2iohlcays.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2yiskbpmx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dmkwdyjx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rzpnkftw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2szabhkoz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yxkktepe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2sszuovzk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bieqgsje.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqnplddu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvrraote.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqwedotb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbrgshyn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2npkdejot.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pysmjppr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rpowouvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sxuzvhlg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dtvtcdsz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xrlpgsyv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zrzcarmj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2khlzgjhn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wkvxlnhp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrcaduzt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mtagajah.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lboawpde.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sehmjkmq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vsboxiyn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bkzsttrk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbjmfhrv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2meqxswnk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cpncnwpa.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dkjalwmr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zaaxddsc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qfuibqsa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wxznkqib.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wgcharlw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ltciuasx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2whfbuhoh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mhfnlduh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzyqpfbn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vjvsyhsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cszhnohq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rteiefis.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ooyluexx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2btvyqzfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2isotlikg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pchdcpad.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wnjxmggv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2atnfbbft.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lrtywsvd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cpssmsvy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cfjiwppo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2opiwiozs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdhosvk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wssolkuk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqxvhlda.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dwfkqwjk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ancebbfb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2booujgot.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ftpvgxwm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nzuzcwqk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pslesrtc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2usjwrvoq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2equpvllr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ksrsvrrx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpstplvh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vroijnsh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ucbchcgf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xthbctpe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjsxdztx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yddvnatq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nwamobgp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rzpyqcqw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bxoynzts.html


<!-- 参考信息 -->