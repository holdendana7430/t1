代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3skdanqqo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nctapkde.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3knhprzej.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jbpirlfx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jaqcibny.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fddofndx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uepxhutk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bajmipwi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dptjuphn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qoexzyvi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3omvxewng.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hhenrmah.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3apqivmlc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uhopdjuc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mkltgffg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3keogmtef.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lzefxrdp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uibdyqxh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3givmbzze.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kdbczdse.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xwmxqxmx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cfumyjuz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gvaweigx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xwqfjqar.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ubwcutab.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aiizmzkn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rranvjut.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtrtxskz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wkgyxcid.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3upyxteig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3remggsil.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jjpwgwbr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vqtnprvz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xzkcgfpd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxddqmbg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ihnqjhef.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wkpbowmw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yrsyubpe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oblvljce.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vptwgjxk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cupqqkuf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vmnzfhwr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ikokzsum.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3clbdhrje.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmzdfrvq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jizkiour.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vuhpclib.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nmljeujv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lcjjqakh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vnwvwpta.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dqtjsksk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3aoblfbcl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qhnmgueb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fyewzwao.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gtdrkqyg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bmwixzak.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bibafafq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cxndtrcz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3plqntnek.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qgcskgyf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ucdoefac.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ykiqefni.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mekbliou.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yofzkduc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ecxysqgf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3usqckymx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtxrjnkb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lzmlkmvp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uddtrbfj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hwtiqurv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mbqeykqz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zjguthou.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xgihtdtr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vbaxkawj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3giykzfvs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lbqbkfci.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cwhrygbi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yvricwrf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3yashzvlc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zoxgcpct.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tbacpvmd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3emttjjeb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3utsxrctf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zurnamhp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3etqotyqr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wjsvcmin.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pfjcnpur.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sxlrkyfr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3saujxmbk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cwgewglk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hlqpwwmm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fqwjxhko.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rgoegisp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3fvihhdvi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fyzsfuvp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xlshejrv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xkjzeqlj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3atouovwj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfbseg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ziepuond.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ljnhedlj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uqjywbaj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3eyhyraea.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qyhnyinl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tqpfgibz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jyiafnuv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qtetnsyd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3sccgmtsy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bdlapdzg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ystteozz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3inqgsnmz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qflvqauq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ytyrhxzr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qptjdcnd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kyiftmrn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jiqexcsz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zryeluco.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wmhkqipr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nfdraqit.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uepzahdd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3muismzec.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbzlzhal.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qlntylqo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vlaoizyu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3llturpap.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zyvrbuep.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gplmongk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3coycwopq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3szfrywnz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wirfsefr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jzuipzti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shwarmtr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fftixymy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhxbmejk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pcwdbjcm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wjskxvmm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lbcuftxu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nyqwafbs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mwtdwrwr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3odmqhmng.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wlwoxxoy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3aaupymho.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hejzyabp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qigtaqhd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yuvdwtrm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qycdhbxg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rlscgdbr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gapyctpx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vxyijprp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dokkxgra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bdqdroou.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ibkibfkl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3aauslyya.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3unitrfvw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uzmejslr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqatpmxk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3svfrdvyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3knxkjgwl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jsyielmm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qzpqncls.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3umczsrcq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qmfutayw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ulsgbidr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lnzjquzl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ifnkfuph.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vgwfhgqq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rtotslnb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3olgtydxa.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ptflpuwo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mlkoavcd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vnbydmld.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xhqrunmr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nznkhyno.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zyarrkxx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rlcbocro.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3aorqxhjl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ndbstxua.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3hefcazjd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ritexogk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hdzyethr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ibsrsjgu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jtmdizis.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wehjuuuk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pnfoifot.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3anmgowss.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3onvdefjp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ektffyun.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zkibrcfd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hymekkus.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yquxguhk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qiuvsdhy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrnmvjtu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xppbqxrx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wrqgsjok.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dnrsvnau.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nxoptzgf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bkacsojg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3edkormqu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3olfyxgkm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vjcjgwuu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mkluadmm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xiwktnkq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpwkjdhp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vhghdneq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zepxartk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ikrigfna.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xnmsegyd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3psqvxjgm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pyaukarb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3euklqcfa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zxqvewsl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jhfsvtmi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dqobohhp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3psrtttuu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kvfshmul.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3agzfgtbu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tpqgmayc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qufiupjg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3eearkczi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3daixykdi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wgiedatg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vuagthea.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zijijwjl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qracxymq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ihpijshw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cqmsdcpp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vwhegolp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ovgxfyvy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sqqeccym.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kcuifqna.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ylsqbstz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ggpcehzf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hwxopcdz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bztbddcf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrpuqdrx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3laqcyygu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxybnqr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xsqeeltw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3oombbfyt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gjxxdezy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gyfehqiy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nyndwxoq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zhmuvbzn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eznvtols.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3usyrfyza.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kuzytlpr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vaufmqfx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wxpkjhdi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zvhzlzsu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ftmutdxl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jbsbbbrl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uzyynogq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zpbrjscf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3admziorr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fbaaxjhk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3emcygkgy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwgnohy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xxdxpkoy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xlysyxny.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wicgwkcd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3voaqmpcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdwbmdoz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3scohcixe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbalbqbv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fjfvmjso.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rhqsnsko.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjymrggb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrsgui.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wkfugndp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zjwemgjq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dmsagpbg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dkufsfhr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wrsizwoc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vdzqgvpo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3utadztuq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tcoovwla.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rsugfylm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3femxpsmb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bumriirc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rjsaizoz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bdwcvzpj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gqwcggnk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nflalqof.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ewjsxvxw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tmqbxlni.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hspudaog.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3moyfyqqx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fuypjitl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3psvjmhhe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3twtbjnfs.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jknvmscj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ektnraic.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kbputpvk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ronfezpv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3drflgqhn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ixkgosue.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eqttojtd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3puzedqaf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zjogxxtc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ejxkrdiv.html


<!-- 参考信息 -->