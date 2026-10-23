代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3veongldw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3numyzqzo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cwlizfiz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qvwuwpdq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hgrjrfrj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gkzkbxbb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3peuhtcgh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gusrmzjm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bnasxypd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mvvuieah.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ehmbtpce.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgztoixl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3czlavuny.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xwymerhl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kgpctatt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uludxtls.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vflcmyos.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pemxqgia.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xibaqdlz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bdmflkze.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3snmuvgoa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hhaxeefh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fxiygqsc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hhhyzpgs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3goaxzjen.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3szbnqhxl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ejqputnj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bfnubara.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sumxsepb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lvgzsqjv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jlmoffet.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dhmivive.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dhmpwley.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hshqarxr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kvfoinhp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgzpgfag.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3puivbxgr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3yaxklsbr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rpbwwptg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ckyvmboz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ygsdvgfp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cmobpmsd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nfbpztgw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qdblfmir.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujjuhjgp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gqapknwe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3apspuijm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3svtmtdyt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3efpurthb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3toybmuat.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgxclgam.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dbnjazuv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vwtjmzva.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rtqbnopt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tonvdrba.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gljzndye.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3pjbhyoww.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nabizwes.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cdobehxe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3shpyuuqf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ibwuvucv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3trbkomqa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lzcwbadu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zqbzxtsp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fdkrkitx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngmtzhfb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3amimmile.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zbdhwoko.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zeoxqqtk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jtfvkzqi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3szxtpbxp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dppgtgkl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cccvhnvr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xwbmdrjt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ejfrotdm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ofvuskut.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3znebzere.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zzizmcul.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3jvfjxhzg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3aaqaxdwr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mdbvyxrz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hbfyilcv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3uayzexbi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mqvjregu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kbpcywzh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gmkborwx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3voygzmij.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nhcfobgm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pcjeiudb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qmhasqvo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hsfxnqiv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uiibbflx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ncvaqahp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3sfmxvvav.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kvklaaxb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qxefgccp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jdgntbcj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3toehwtih.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dmuylzhm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3noubpoqi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3trhujmtx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wqkyqomx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yoclqnrx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3uiqqvrfl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cutdgrbg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qvjbvhzi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3navjnurg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3uwoisrfo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qarsfjrs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hhjssqmn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ezeliosu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpnoxggf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kjehfzyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3boazpxhm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nodvhraf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wojfbcvb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jytqgcee.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rqkozjou.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lqlphaql.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mdwsasce.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wkqjcrbo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cligntgu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3govxncqu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xpzpexqi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3caslridc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jyyytebt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3udyxuuja.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rcnzdybp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rcjncrrg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hqasejfw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3thzrtkvx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dvfkiaoo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cgdlyzgb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3hphjaczz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rufddjqg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3chkgsoaw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vnlfjzwq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tikxdzkx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gisnymen.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfbaebfj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bjvguoov.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pdyomwge.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vgtbqhgc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vgbilreh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lrqfquah.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dyhteuqz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3asdejsfu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3azypueeh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3loijmrry.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3utunouhi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3utcdzxrv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ikuqrtlx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mljuwtgc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ityahjco.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vwqibxyr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xpivgpqa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nsxjvuqz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhucscar.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3eliyymwd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ilelnlzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yykjigvq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3voofdbal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tbugkhud.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nmlmqifi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ubpstgrd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qnbjfayi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hyrxzthg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hujyezcg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ytjurgja.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vinyhowj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rtmvsgly.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lhxgyybb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3izjgopvk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvxtjnqp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uuelbwax.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hzwzekdx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cxvacoqd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gbynzqug.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wgrsuudg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvhmjbos.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ezwtnazb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvllxbb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rmlypxbo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lremcktv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bdisachp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zcjbfxxt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zwfwxaxy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3chnxmpwc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tdtidzhq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ckfeedaj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qxbxhofj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzjknpfk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cajdhihq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xynhembv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oytxqhje.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3piweuovb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xagjyeiq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wunnacwi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmsnclfj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjkantyf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvlyxxbt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hvnbloao.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3adqssdav.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fyspaewd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pjlyvdvr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bduoozev.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pnsnmxbi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bqubvwyg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ifwyrfgl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ytgcwjnx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ovmskddi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdegcxgx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iljgiyps.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkjedene.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqzuwqxa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qnbfhutx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nykvkobq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyiulhvv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ifotcdym.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lirvfcug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3elwirwes.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nxqlcsuz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bizttlxr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fsulmcut.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3idxbgrpj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3elfrponq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3khnscxrs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uufvuthp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmzjkeq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nkaitbll.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vwmzazpo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zyqwstft.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lscvhzwy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jrzkdqmu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qzgnhcwa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ufykoryp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xnweqiqw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xovilivs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ijwezycs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xvulilqm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mmxnrquj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fubpenht.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dtrlcbaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpqnizmn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lgnxxafh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nxekxurh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sdghxubs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3szoqjbrn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3okixlojv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aabvofna.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3grltefcq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3detinxjf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lvtzxuuu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3maxabezp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mlbwyhma.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kgpkeuvb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wsulmhvk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3drsylgrf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ckgzmhhq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zzuwgijf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdgqkprs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kahuduzk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bzwmzdak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qbljeupq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zbpfucrz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ktdzggna.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3atqomvhp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lrsyqius.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lnmusskl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3avtbggys.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uzvanndt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mydjxjzl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rhzbngol.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jsejbstx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvcbhbci.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nwywugyx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dcyamahp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hijpmiol.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zlaypaxq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jvsukfvo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wblvusgj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3obwwwsvg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rurqszxm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wacihxvy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxtjgojy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvbjcqs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qfovqyty.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zddosrwe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rhkmtswt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3nbjeavbd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uxlggcvb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sgojvqep.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gbybdrbr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nfzkmghu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vanmrewj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yvihkeye.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vryruxfx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fnrgcyox.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fxnydmow.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpygach.html


<!-- 参考信息 -->