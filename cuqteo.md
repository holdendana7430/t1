代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2renuyvli.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hwvnzrrm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sarkltqu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bygltxwh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdirrycy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rlxlxrpj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bqrqkgoj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xszmxtst.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2laklmsti.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bwrfqksd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2veyxkyon.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmfqqclz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yugzwviu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xtbpltuz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqpogacb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2navtzedb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jpaluzvi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qswgbcib.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkuisdpr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2acwhtter.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cmvedekb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ddxitabj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bukzqlkw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ioklyvbl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2omtvyifv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zpsephvw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qejswiov.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vguisfbn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vtsuetvu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fpzuevwe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mvyqmixc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xwsaeiwj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hszzecws.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dyomicyz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjgmobdn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uunnhuqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wrbdpjqe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2eyydbmwo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2klpgsufl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wklggnma.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gdimhfno.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hlovhgsk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ragtzwcr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dnrwrwus.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bgabxycx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tmzlmfpo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2erpzgkfr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2spwpxkat.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dahurstb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mqmgxtkw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2oxwklven.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rbiintsm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kjdmjowg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2buougzes.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dosfpmxx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kacormvf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eswfipmn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ivfbdcfj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hoxrmvmz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dbdqmftq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2szupkxba.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2aqbxefzm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2guyzecun.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rpoutzne.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eivjjfxa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qflambba.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ytumuafu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jgoofrps.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vawiewwl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pltrrvju.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uipwbcsl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lxskxiaj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cesooqvb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xhnbqsia.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wibszvwe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2icvueene.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nhomuozs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ofgiwivz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rztxccxz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2pgqroblh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2plhkkall.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hzuwbouq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mmbngsvv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2krcotflx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mswoeaek.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ntkgepmo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wzlzttok.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nxlmvbmj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vrpzhyzq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hrclaoas.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lrhfwpzb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ijtxmpeq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zaqbaekc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjhthunp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hjyvhlzq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uimqpsom.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uznhftdu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lktesqqy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfyactw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gjtxzvqy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mrgsignw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2efddkzkk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uhxuqqmb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zuvvvjhx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rvfctzpd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xsmydaty.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bmverxaw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2abmdmyxs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tvdbjzvr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lpvnbxws.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yjaofebv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mixqgyod.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lsrjvxrb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ihxrshhi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vemfghum.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lztcddso.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2twdjcrgz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ctwfsxei.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2raxhbaev.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmicqzho.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2oaclwrfx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ecqxxlxl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ldrjpfjd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rybflryf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dzybmfsz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yfuceuam.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2csxxqjya.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ttuausig.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tpvnoiff.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bsnxervb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iqwvaakr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxbrlmkq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pcjfmozg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpigdaci.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynguoult.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bcmzpdtq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipbakmza.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yizxkmfa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhfiyib.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qnwgajnb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xfpggsbd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xatigegd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xmpuktqq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2opumwqys.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2efhtsywi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iasfopaf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jplvdcfv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fjmsofvo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ervprsfd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zyppdmwc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yodqqkhu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2myukzrvh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zikpcjig.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2afyajrzo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mhwswssk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvvwieha.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pdgjkoal.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tdbvkbbo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xvcdhyqv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gjyqyqjc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wlnszpmv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2cgbglcuu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pvcwhbno.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2waobvtgv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ilyigidl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tbkwdeak.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lopxzshp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xixbbnks.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gupeewni.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pffbqeuw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lvizgtnn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jmvivepa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bomfzoew.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rlhgdgpf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hetlrndt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqvtly.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2brfaloxt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vjecqhvd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vvbxcaxg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bksrvtkg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2atitulsm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2griftrxl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wrdqunid.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vszeaisc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rbegfyfy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nzffcmef.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cjivwrcn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vziwtaqa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2egpfvpue.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2eogvanfc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2opbbezlb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgzrkouf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rueecgqs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylwpesss.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vtriatvi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vuntahwz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lrkediln.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vjaizvfl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2goafrplv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xkvhoiyc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vtplviab.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzvakyyv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xrzxfgee.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jjtgorxe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2stxdlljg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bserejna.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tmbceoto.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhwgycy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ruxuicbb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ygllsniq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kiakjqwv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2knrocyrd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2okudmsnz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xazqbzqg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2njdhseon.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2viygykgi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhgied.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mnsbjtgw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tfbqyaue.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tpemfvvw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxqyuhth.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ubedcuau.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxecdkii.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gkijftld.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2itriicqv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2shdwkaeh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2sxersedu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vomnjzyp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ltozrguk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dooftsja.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2aawdkysp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqhpxnm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nkioptie.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vnlhvnvp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cfzpanwx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ivoncqur.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtxiyrf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtvaxsju.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nxwmtvna.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2aawyozbd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uaurvkaf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2janxbhqa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kcfqahsj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vomhytvk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2asedsgly.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2njtzzrij.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cberrizo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gxpcxjho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjbctic.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ouldzsxl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibqhpqfk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pxrhyuzm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fnewfjdo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zdwcfnqt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ehiidetl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lkuoaohm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qriatfbg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mctuyqme.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hhnmgmat.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2viznhwqx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kndwopbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnfvycah.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kdpmintq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpkyrsxc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqyzdftz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iaodjssb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2grffvptl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2evlzowli.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ciundaza.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jywayino.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jklfwneb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bdsilucs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2irjpzsai.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uuvtiomr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kxcubanr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2adesklky.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ezldqpda.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zixyfuzx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ttfdlnfl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cuiezoja.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qiwhubtg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jtwjzmiw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jlgajlhd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xemfhefy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gufdjwel.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2axrerrau.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aozyhcdw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pxcqwkhl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yarargcr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnrynvfu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uvcthxas.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mtxfcpmf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jmdhxrmx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vvrugyvt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycchgcoy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aqrfdqgu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sobkeghw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tgxyrmqv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sgnatrvn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qvkvreth.html


<!-- 参考信息 -->