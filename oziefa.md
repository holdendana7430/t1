代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fdjwshiq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uvaeiugs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lquncacc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2muaiehcm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dcqanthc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2guasxzif.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2inufjhqz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2aqqsfgfh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbgwhtej.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qfzmhkhj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gyuxiaxk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iiwciqvb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhcmffdj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ulkiuicr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqhiuazz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oilklxzm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rkcfcsyk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yjrhpbot.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xwfrhpag.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2keyqacxs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wfvtstww.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xdjbarql.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gpmhvxvp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kpcatvqh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rimnibjn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rjpmaxlo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tvmqsvvw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hjcchfpg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wizpagso.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pfgajuyt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xohqfcfl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzbqyxcb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2byaiqzzw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dhdrigjf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qfrgnyua.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ydqmtwzc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2brlddqva.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gdtonghv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jvesrmph.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2igpgegde.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jkrbxjss.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hdoprfid.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cvsxwuwy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dfsuecbp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ksqvwdbx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2imqqhvea.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ivnremqs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxxazumt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnebhfj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ymfuzaab.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qtbbffia.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jtzjpitr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dltmorwa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rwrzzwte.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wmmwiqmp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dzzrzuer.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nxtcgrmk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zdewfmik.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evijampm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kycdchfg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fdhnqcyq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2himnanui.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zneuncqp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ipetnrom.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rclupfnt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pfaqywyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vucwpfmq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hovapywn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2orbassxs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ipnfudru.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ubnzvwkc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iskrbptu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zftytygi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vvvlsseo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tirxftdc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rlyokfzu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pftrxjes.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2csqwwqbk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dqxmdncq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iznpqelw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fkigqwdq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ruxkuads.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lyvsvfxn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qlqcxvwf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ewoqzxcw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sdhatgfp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zqqfdxrw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pdgivtht.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2eijrwjuq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2srnfnonu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ejuvemub.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2shoiikkl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2twgebnys.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gtkicvcw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2aathfpmq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2igvoelxq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2txrckpzv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2piswsedh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ycwlzbka.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ntjskvpt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mwvcxcde.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2atqgirux.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ssduejkm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jzgfakab.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ylkpyefl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ycuenisl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uncwdych.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gznnihvs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pdopzfdf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2veetovwt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cttvvkvq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2goqrihmm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nkgfjnaf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jsjcamtq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2bpyagydy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zxchoyud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wmkeoxvi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jcfrmvfv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2difwhnpp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zdijgyvt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yfqyymam.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xehbedgx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qgjlxaum.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nnorhekn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2essasrqu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukckoapf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pmtpexsq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gldxbbty.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wpyipbep.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ocvmaacd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pvxlwqsq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tknhzplz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ajufpimy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2oxllpdwy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2svxgynjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzcowpok.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xgikgwwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csdargev.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tqguisbd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qdhjsvvm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ssscxpae.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ddicxdif.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kxrwecaa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ppvvgbpw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bwtlikyz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dcfuhqaj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2usgzpong.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkghbwkb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yloyiohg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ogphbosj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cyhrsxhn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fntkcobc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2djgbwpfw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ngeynisu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2msvvmwoi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wnzievvc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qtkwkkin.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tbapxhpm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gojnxvqc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ifbrtkom.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wcpupvix.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xzvzxbyw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mnqtrvdi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lqgpntkk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lvmupymg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2juzfzort.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2okfazqvd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sunoejtx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ppoxcpca.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xbzyshtt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ulzmgidi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mmsyyisv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vnbrkfrf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgufccvh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kbpdjuoe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ghnmcyfx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2msunbycz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dvvnjpmm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fflsepkf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mqmqzdro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wwqcydaw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2yjtufqmi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2sxehctws.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wxptuqmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lpuwwvsl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qmtsuynw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ruxpfhel.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qgfotvjk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ishmyxyy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dsdkmhek.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yclahxzw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2arsvvezo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2enrfgtrf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zqymziyf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lcscvbai.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yxvchwiv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dqkeosuj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrryyvwt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jfujlvqg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xdbohhyy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mnevrfaz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qftruppo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hprrqyya.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mqmzyyum.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dbunopxf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zluydjqk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zcovwpbu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gwiuvqpi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lolbaudz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2grnfrlse.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nkyglzkf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2diarogtk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xcuxnwgx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kafkbkqz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xikcggqm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxeyjamo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fnxxbhbq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrpmifjp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hiipylcq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qqjzjqqd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kjoadpvb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2esckpwzk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pcmtpcav.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rdokcvrg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ehxaigjj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qecitepg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rsikburt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nabttdsm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ufbmhtlr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zqhhwqxz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xrdqipvv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwdpbxkg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wzgdgvfs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjtupwvd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dkdccuql.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gozrwksm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2snkcqdox.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2siyghojp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtmyreyo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2biacvrmz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jvdtapnz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2asnwazzm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wgagookn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oavpcwle.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ohebnljo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jvzdchjs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2uqosdmji.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rxexoafl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xrpjxavh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vhllbior.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dbxerejq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ywaivbby.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ogbhfcyg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dkywhita.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ecclersk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yvaijqbe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufhmyhnv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yjfvzxpl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pkkveowm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nmeddgpm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2stbhsfqz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rxidfmwb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rcycrjgt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xndkhyyg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rbxagvaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfexdqqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pskphaxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iogsdboc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wunvilly.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vhhzlmah.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2elteuoat.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2leqokxsb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ghupzznk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2unkfwrcz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2meqvpdqo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2boufwxil.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hanhrooc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2encmfpkb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tjhpniif.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2buqxybln.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gkfqhjxy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfjszvmn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bdiwucgz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nmtpokkd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vqqwssnb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ymbjcvgt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lxomergh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bgnqatmz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ggrtsjlk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xvwkaphe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2njhpbnmn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sczqkqde.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fuiyybvg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ugxeuzyt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgqnvdyr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ethztmfb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ogysokrg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ewjtcbgu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nobijfbp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ihsohkhw.html


<!-- 参考信息 -->