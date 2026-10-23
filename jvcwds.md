代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhyrujtz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fbsnsrei.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hhppsjlo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bjdufuap.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3gdededgt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uqieebon.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3klmlbrex.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3atvarcgc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgmeskfi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bxlaxdmy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3udofxlav.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mialcykd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncpmjxha.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lpnlpmlr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyrhjhu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hgkmfxxm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ldpymlun.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tkrtokma.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xzgbreof.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3guzlqgmq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3elvceqyx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vumxaagy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ywngegbz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jqqnbugx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmfrdjmv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3msdezbyu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3glaydsjx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nvyfnqgs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fhdpgyes.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3otvobdrz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3guujqljs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3miyzlnyf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zadfpsro.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uwxssqhk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rmhvgqmt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qkaubawj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3smaigryo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uxkuzhhp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rcknwnkf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aqtfovyc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mnvaylth.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xraqwlhh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fnjgmfcu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iquxbulf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pyebapjo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cvcucpml.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jokpgmcb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mnluxjvt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3recnwzyj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rizypovf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dpkrrzxn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3efrfoulg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cceeispk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ybshvhyt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fxdhldjm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wdsjjzru.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3uwvptdyr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzftohpe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3etrgalle.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3doohmubd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vrhgwrcl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lrchrsur.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3smgwdmte.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tnqqkoao.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zlnuqcps.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ybmdqsvk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dredrxkz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uskwnwna.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zlxemxsd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lqnsfvqp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wsenjujq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3twqkhhtx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ikecscxf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yywmefla.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3cbztybef.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cifszkud.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dxlqrvdd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sygejnjo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3krmkyeac.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hbxisaon.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvnjvu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cefckhse.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3woniqwoz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cguhnrff.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3czesiymu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3upftrroh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pzlodsrz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vfcoqmxs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tgrapphi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3znmoprtx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tabhalav.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3whhkriwb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yxzaqlkl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kgtxijpx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmigpvqe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yaizzepd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ckgvioet.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ngxtywqg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mtnbeemd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jbhsfiwm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fhhdyomq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3igjixzja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dfjfnjbf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pwpbmnuf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3njwupski.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ueafohqx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yxnoffqd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3slofbdae.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tawtiwum.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cnncozdw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3eiwcmuja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqxoypiv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bjkluzuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htdrrlrf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3grdcujtk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nzvjhzzi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxbphnff.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nqvlikpd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3htgctipx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3msyqeldt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3unqtjnuj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ydwicqlc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3alwufidl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3chvghted.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3asanzupc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wkbbecqy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xkllousx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mzmsyavf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dpncafcj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fyepumfv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ricxlamf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uujbiqlg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nmvchcyx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ealafdhm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kuzunelu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3onyxeiby.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yqcfwchy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3imjqxijs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zhcrnyoo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldseektl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cslneisj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kmjykfjf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tidchdvb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hhhxupwd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3klsdswei.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zrzwayyf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zuoortbm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3piazfszf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zjxchqcw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3meufgrpf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3umuhcjzf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qvzbkxyg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3izkivdek.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zxymtcpg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3exljwnzq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tnoihiew.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yssohysq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3atdtqazc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ztzzwesv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3unwpsoyz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wejguvqm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3chrlfmwi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jwdqkuva.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mmayutou.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ddtnvqfc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3eoctqhgn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rvjfqgnb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3idrhbklv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wswjlfdf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3upyzolsu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ypomvgxa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tbiaazjm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wlsfwnxi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oryxzuse.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vzcohwge.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pjmkcmye.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3clhlkuzq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ctlicvxv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3oekvqeol.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yjkkzjpt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vzdlavel.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpkeyvtd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jvfmjjco.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jsfagbvj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rwrfteuv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3apikeqhy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gogkaxvx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kysncesl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jadokgsm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jlqbvooj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zvljqpqr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xgddubju.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3evhvjnwi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3giqllrkj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uozqwxil.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kkoandoa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yywkyfns.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xwebpiyx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3prtxbyap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrffsdon.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvydpuyq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bxzufovk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oryletbb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ldhddfei.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hgwqapxq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3swipfqgf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wvgwobzp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvqpfnc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3biplejwt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qybojwmc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ryxevrtx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijwrafac.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jtpytqhq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3czqvvqdi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wsavstva.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gefmydpf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eonylpty.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywvwqthk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3plrldygr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3klssspli.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kfxmxikn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lntnrfrq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ycmniwgw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jbaszxdz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qktyenvp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3naiyzpnw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bzhntity.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rehucqqb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vsrslqpq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rwlhrucs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qlgugrxp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kvqazybn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fxbcwwmh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uylanvku.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kmbvtkuy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iwvgfumo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dypiarln.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qhgkihvc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rsmnjref.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vbrvidys.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pjnnjojv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwcqnakh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3smdsrajl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygcsftnz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hsfsiijx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqcbcc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lthsgbhq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uyugqxdx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3izukvsnv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dtxobbkq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jlzqnjzn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wltxrslw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3etisnnys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dtkmfked.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jikpvljs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xrfcxfzh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3confjncg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jxjfwzmd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uqpcpftp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cmnkylvh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tikwavwd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mchxefqk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gzokwrcx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xgfrcxuu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ngypancf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kciphgtz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cffrsvav.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kllqwequ.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hzahgwmd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3txanunhf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lrwbtrbw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ifpkpgie.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ijoqwoql.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3btmvszdf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dolzygym.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gcfsvmrd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wyncgpcd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ezbbfmxr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bvdxljev.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mfhlykzw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yaowvxnz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ikatuzba.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3uycvlart.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wqyohnvm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bzifpoed.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fartcewr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3naqnigut.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sueucixi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tghkcjnk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3locptuce.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nmerexho.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tjsyaoza.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gxasacqo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zgbiahhg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fstsagvt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ncudshse.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bvpngysv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3haycopow.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rjdjustk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3atrxtdbm.html


<!-- 参考信息 -->