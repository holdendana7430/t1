代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gzgeyokvs.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gvrrhodch.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gyugryhfl.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gakdrczde.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gntcldkiy.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gfhwealzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gkmwlnjel.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/grtpucwcl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gemysqxyg.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gndffjbqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gwrtyogoz.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gelvzpobr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gbvzakcbj.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gbaufbjur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/guveypylu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/goyjqpizr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gckeckwyz.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/ghutxtbfk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gchszxnyh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxjxpsypc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gjjodhivh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gnlvqcikp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/glfjwsdfk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gaadhnnup.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gixsanqfp.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gatyxnmzq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gzadupygb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gtniocnjb.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gbibogchw.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/ggjtrxfdu.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gnbkcuzho.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gutiwtbrh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gkznuxljo.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gsjvdnfxg.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzvcnwmzo.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gycykhadb.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gkpiqvoqg.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gxgqpvwcb.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/ghqqhjdcc.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gbhqpfpws.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gahcdsfjf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/guajfzhrc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gvvjwzoql.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gaqbmjuea.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gpvdhakgu.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/ggyombfad.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/ggfbspkyz.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gvwolwrxs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gypnjhtkz.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gyqgyqifx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/grwwzlhdu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/ghvaozklj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gzthomeqh.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gvpmzzdjb.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/grcdffuca.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gzmytfyke.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwffxxicw.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gfokcctcy.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gybzepgkb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gtksdzden.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gpjhmvojk.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/guvxbqmrw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwmtcpn.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gmcjfdylf.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gzpjvjzkt.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/guspjdzgi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gwqnwoeep.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gajazygud.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gsnumltny.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gswocywek.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gutrxcigo.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gyiffvtnd.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gerglyzrd.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gkirhtpjf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gfesznyqo.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/ghhcajouh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gjemwndfr.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/grgckhxwk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gazktsvhn.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gtbjkcjfd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gjyhezelp.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/guovnjqnn.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gswxobhqx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gufekoyme.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gwnoscjfx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gyttthdcf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gmuevgflv.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gdwttzoeq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gagayovll.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gedlqrgjb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gbgndhuho.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/geslmnjpl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gqnqgxatw.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gitqaaqcr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gzsjynhiw.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gkuxjlmnz.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gjppoqszo.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/godqbceqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gnwvmcbvs.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gdlnbrazy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/guujquvup.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gfphwxcmu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gubyxlneb.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gqxtescaz.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gewahaieq.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gyjilwgik.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/groesmdkj.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gldvkhfid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gjzwnyhvt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gbemrkidt.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/ghrxzpvzn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcghwuonc.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gcdpnonkr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjgsgbpwl.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggolknllo.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gmbiiustk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/ggvipuwwm.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gfdcmwrfo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gyavgjccy.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gjyrrnnfc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gjbqyvimz.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/grzsalfro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmnijvcou.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/glaumcovk.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/glwxlbizk.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/glfyzuaiu.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gsxrojmuq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gogqjmxtq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gjdosgpat.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gjjmhvkmz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gvcfffzyf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gsplraxqb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gsbozuevg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnogyvm.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gmjmajlnf.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ggywcojhz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gzqrkczby.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ghbjrbjuu.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/glqcyybww.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gsxtplckl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ggerjemay.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/goktdavmm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/ggfhlzvti.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gdrhayipg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gnlqwycjo.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gmeevccts.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/geiqknsdd.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gygpxmbvj.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gapyrkhfs.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gitmxnlby.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gseluzdon.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gjnytflqy.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gjnnemikl.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gncbtupat.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gaswgszxj.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gvkgltuey.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gawujbbyf.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gaggjhsyq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gotyjkpgd.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ghpphuovw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gdupafxlw.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gokgcpkuh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gcsoqayvw.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/ggqxinaft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gryuknfhz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gxagdqzed.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gnfpbzyhu.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gbdnnsiik.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gsumlvelk.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gkuxbljtx.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvlbtoaoa.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gdkemggac.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gvvgffluw.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gbdkwbpmp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/goavypzew.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gvqkjkipi.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzgsvvr.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/goufacmeg.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gbubhqvgw.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqqvwkuqb.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/grgysmraz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gkqulrksr.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gyxhszdho.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gajrmoyzc.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gpuqngvpo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/godppqybg.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/guyvmgzvu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/ghcogaywy.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gufwbgiur.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxtytgtmv.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gusvunqgw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/grntlofam.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/guiiqoict.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gizaswlgf.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/grfacahba.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gpefopsvf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gqmvykmhn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gyfvrzlcu.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gpieexwet.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gfoevfnht.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ghfyarqog.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gucraudqs.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gxsrethfr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gkfnlbrzu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gmpnarrfb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gdxhqnzwb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gewrsxdoh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/giioxvlmp.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gwjhtocjg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gzvcukbrg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gewubovhh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvtaiqxg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gszhsijik.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gumztbqej.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqqvqhlbl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gvmmraebg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/grvacswgk.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/ggnugcfst.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gkdljforj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/ggeszqtjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gpjbeywxj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbuonzbfq.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/glbxcjhff.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gzoyavchq.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gpdmruedt.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gtvfzfjwy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gmdneywlt.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gxycdnqsj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gwujpgdms.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gvpnktfju.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/glyfyfwlv.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gjumkkhek.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gkjnlsybj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gsrrnheqp.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gexvycwqb.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gqealyuzd.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gvmgabwmf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gambdierp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gdmrirqel.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gaasztjgq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gpviiinhn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsngoomnx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gtwlggvjr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsuijqwcc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqhsyxqfb.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcawpmpdz.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gtdqqammw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/grhwhgbqm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/glmznpzci.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkjrnjgwe.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gxnvktads.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gcurixbsb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gbevzuapp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gggatwocr.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gokvpcojd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gtncggcqs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gpjlfskor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gemdrxwxn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/ggkqfdzxh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gpbfogwri.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gneaeamcx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/geculloiu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/ghwgtgyls.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gytkthgrp.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gjbhibiia.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/grkcytlgs.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gpwhzuyyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/ghvmfilku.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gqzaiuurg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gfqorpxzm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbnpgzzkb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gkrjhscec.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gyhnbdxit.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gtijvvnbh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxxdczowi.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gsptwjtip.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gtvaufwtx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwnvibfxy.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gkkaaqkds.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gggfbgcxk.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gltvtlqqa.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gbdvrzlhs.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gotwjwcmg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/grzivaleo.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gyervnepc.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gblxtjvtv.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gofqcsqgl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gvzctmoqi.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/ghsissedc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/glxflsdkb.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gwrlidlli.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/glfwoewwz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gmwoloahw.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gefoxqprd.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gtvxejesb.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/grrmbpxke.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gosrxcwyw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gyfdyglip.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwcgvajjj.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gzxlmjejs.sHtML


<!-- 参考信息 -->