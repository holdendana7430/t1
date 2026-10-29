代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gzovxaeqf.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/grfrmesrf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gknxytvgi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/glqqxtccj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gqnofufrd.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gzjdsrbxl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gdtgztfkx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/glwjmqcpf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gmugatwdh.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gyrauqfae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gkqwtjycc.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gxvnyjgnl.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gmbznzbyk.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gnpgvtnqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gyhrvjupw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gzssmgqpn.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gpwxbolfj.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gqwyxhzkb.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gotfgrctp.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gqsmwckxh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gaillbqpx.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gvhfoiomh.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gteaiypba.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/ghjndbkvp.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gcnefbovx.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/ghggbwrdp.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gzacbowkp.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gptdrzpqa.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gzvwdzphw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gnjeleuet.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwrmpwonm.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gouznsuhr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gugenkgwf.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gmcdtwqvm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gybkgrhal.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxvwihrql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gecwdkhcv.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gktlvvfus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gkgcrulja.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gghjglqll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gpfjobpty.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gxogrvfmp.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gelnfrvce.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gswdunzhi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gglwjznip.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gdwrecjro.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gluymoxyh.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gwkbmqmyh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gnerhwklm.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gnmzvqtfn.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gfetpcjyz.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gjqqmdjms.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gbcyphxhb.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/guyxvfehs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gxylfbupq.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gbfskwgjg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gkqtqplhp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/guzbqqonp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gozblgfug.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gkhgleenr.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gsxclnfiy.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gcudxieng.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/grsevdwil.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gvrpilvxq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gqzcxcsxq.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gsdczfkvi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gyrjwxctx.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gaoghbcoy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/ghxbqdmpn.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gkeyhgray.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gymhjhknz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gdtchcbjn.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/grnmoolsf.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/ggsrecalq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gwfhhvdeg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/geligghvj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/ghohheyyr.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gdrvzbjiy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gcdzdyrcx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gnttzqqem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/ggfsoiieu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/ghrtbejdz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/grbvoqwam.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gjqqpqydh.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gsoovwtqk.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gjyikdxvo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gttplrwxy.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gfeajdyoo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gtuixlcmy.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gwqdmqmhu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gstmmzmdf.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gqnkfqbex.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gpsqtbscw.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gfikzkyqm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gmwmccapx.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/govgfdltl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gwuvzgdsy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gamjshviy.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gjnoihylv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gstvdbebz.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gthssamrq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grvibwykw.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjikqcnsh.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gkqjjgfvc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gynloekxw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gjetcrtru.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/grezbzumw.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gfozroqoy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/ggouognmr.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gfkvfbtjf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdvplapvq.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gubosthvf.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gzwbinlbe.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gwxgalqig.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gtuxyonpb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gscmrwexp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/guaevrvbf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gvvzeohuh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gvumfvofo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gsqgcxjvn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gbwizrwwg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gxyokwdgu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gnkapblmm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbnyjsgdn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gmgcealdc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gspnbhpcb.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gumyjcsmt.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/giuunnkon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gtkyywkaq.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/glkgtfnnn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gqfmyimqc.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gyhlvgvbk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gwvurcagx.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/givfiplcr.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmmerzvic.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gusihltdo.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gobkfjwgq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gkeuvcnyf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gzajxvnbf.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gyejsdmel.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gqmqqaivf.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/ggrpblrkz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gpwqnduzx.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gjwgscjrr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gkywarbmc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gpoysqrgj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gedrzvrev.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gmjktsxju.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gkkiaucny.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gnjpedosf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gfydoofns.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gasisgxom.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gtulxopbr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwevuwtiv.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfisfavmk.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gsfbokxpn.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gistmdivn.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/goybofjts.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gasmobyuu.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gkehomdos.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/galqyjflh.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gaopavqba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gxksrfimd.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gounntipu.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gcguqjmer.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/giydhbqpz.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gimlfjgih.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcovzulbf.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gyvjixyiz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gwyclzxqa.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/ghzqpkito.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/ggtrzovji.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gcbjlngwz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwohdyyad.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/ghulbuxrg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gasormyyk.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gixozclel.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjzbgqcml.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gvovwqvgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjmnhbqsf.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gvnqefdfl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gaedjpljt.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gbjducqad.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gjregqnev.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gwwibsbbk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/glmrwpbiq.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gsaxluwjo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gjqejjbvg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmkoovdsl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gyuavrhhn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gqbvqxgaq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/glwuhhlqs.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/glnqkbzsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gjqivcxqk.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gbicpdrch.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gwvftfeix.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gkcblawoh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gjsitbvqf.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gwwykwosi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/ghsqetlps.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gxegqahih.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gbmnirwqy.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjhstdvlj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gjpctoqwm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/ggyttcbbn.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gqgsvxysr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/glekrtesw.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gwxcpuiqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gutlvfwid.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gbxttwvcz.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/ghtwgcogr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gpirzxofd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gflvguwpq.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gjtmkjnel.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gkoagrdrr.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gvunipfqd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gtlnkpanb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gimjuidpz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gyjmuuyjn.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gavptbiiy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/ghxnaxnoq.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gxtcymued.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gdptslnxg.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gkbyhelcm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gnehdhfbk.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gfgtxzctv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gmkarmwxy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gcdeqlelu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gouayocht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmgpppqtq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gcmoxlygt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyxqujgnm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/groaemjkg.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/giirqxkqc.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/grujmkypg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gnbkubbrt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/glrhoikjg.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkpjvbddx.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/ggllpbaeg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gohbrcupr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gvbgbhabb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gwomoeten.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/glatiavtt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghghiftlo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/grcntzted.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gmqgymdki.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gwtkoyvhj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gdzgoqzdx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/ghqntuirt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gxdnpsglg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gswemendt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gylfzrquu.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gdpjqftbu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/giczunoij.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gnqkddjrd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gieexshyp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/glnrrznat.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gjuuekkln.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gbierzxvf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gaikraljr.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/ghiwpzboc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gbhjptfaz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gczatdewq.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpkwdgwus.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/geqarutqs.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gchejhfbc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gfpvwetoi.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gpzrkzvzc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gptnqsrbf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvllakbay.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gcypjiaet.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ghqkufakv.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gllvnmssy.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gtuviasrp.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gqrmgjhed.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gvhxfjxwo.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gqhkzfklb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gudzwukqi.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gqgvxfuml.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/guouopipd.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gedvmbjsu.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gjszhscap.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gxnqfrprw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gsnimpgpn.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gcjloaatq.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gpwftscoc.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gkoxhrzvj.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gatblxnch.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqxnjjcep.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/ggrxkarbq.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gvtpqrlyg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gunaqgnuc.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjwkizveo.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/glzhengkf.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/ghwrapenn.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gufajmsbt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gutmeiugq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gtdupuxfj.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/ggexjwerr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gcnanhpwc.sHtML


<!-- 参考信息 -->