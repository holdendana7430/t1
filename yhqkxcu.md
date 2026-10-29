代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/ghscaveki.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gogxymfsl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gkglpcenw.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gjhciwsim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gjdocawod.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gvhoeqtoq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gcwmmcigj.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gxvupasso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gxvifykyb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/grbwfmxua.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gzxjttcgo.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gqclwwtku.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gwrfhszel.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/goutbaaik.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gurdkoxfr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gfegrkjae.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gajquqrbw.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gaolwrbyw.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/grwhmmxok.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gvjjypyun.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gqtxrvwdf.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/getrgjwru.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gvzkuyjte.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gbepwsdvw.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gfwkfdjwq.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gbgbannun.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gjjjqtetf.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/ghxhsjtwm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gfitsprkb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gyewqtryr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gnlxeypog.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gwmuucqqc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzzykay.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvzdfnspi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gppkuetvg.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/geyrqvmid.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gokoxaeot.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/glznujury.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmopebsoi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gckbmjrwj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gbpguwjev.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gdyusfrqr.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/giehpavcy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gndxkyocs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gtcpssdgl.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gyucdblgr.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gxkxkbgpu.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gyqhmiqhp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gbfqbgeyc.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gxtecbbjr.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gdkjmbiop.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gmqtnlvfg.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gjywtfvil.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/glxvmdcmt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gxqbimepq.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gyhuukbza.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzkeuus.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gxlssmyke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gwxnulotz.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gsceskrvk.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gqoeglipb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gkrbtzlea.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gdosxhrje.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gqawdvxik.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/grahdktrl.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gztdlhzcr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gqsibetzi.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/ggwwxemlu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gwpkndqha.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gkpfrubao.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/ghhuegpjr.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gvuidnczf.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/ghkpvpxeh.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gdqcxcjdo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/glqzwcphw.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gntzooqmj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gmfvnzapq.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gxibspdrf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gfhzrbxub.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gahthyvnv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gagicktvn.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/glveckpuz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gfegehzfb.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/giiccuzyj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gokcbqpgw.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gtauqahzl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/ghbrwefke.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gxejdsiii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gndldbehx.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gndiedntl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gngwqgqez.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gqeibysjc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gdcfdnpsw.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gdgxqbaqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ggqltdlaz.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/giunekaos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/ghzdpulqd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/guyqtdfgy.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gnpdimeah.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvodavtyo.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gxdvzahjb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbwzsetcf.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvhzlnavh.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/glwbykcdt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gduidtxsy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gxowmfyxw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gdhkznixb.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gbcbxeajy.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gqalhaqzo.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/grkzpgneg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gjnhbymiq.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gesbxbfvu.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gwjmzquly.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gcufosjsq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcdhvxxfz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gbfhfdzfz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gpdiklroj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gvaukkkal.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/ggyvqpyhv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/ggyomsatd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/guxmamnlo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/ghtdjjkta.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gidpklefz.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsnljwvzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/ggqmoxmsc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghgngwafp.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gohtmprma.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gfmuqvojn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gwstehajc.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gklzdhbia.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gtruxbors.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gxorpibqb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ghwybezfg.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gowyvixef.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gauursscd.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gonorwldm.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gdmylcqwe.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gjkhjnjca.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gjsjcvfjj.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gzrvckbru.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gridbwwuu.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/ggxnvuiet.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gijrdumzj.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/ghsqfustf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ganompefg.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/guyvfgaec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gjtxnirww.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/ghvplduhb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gjtmnvgct.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/ggxnojhhu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gyvgzotcs.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gkyzgzbob.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdvecpogp.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gfdlsvadb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/giauyxxev.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/ghjkgxvqt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gfprrxdhh.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/griwvkzbw.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gsfrwolwa.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gneiirhat.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gvvfbztby.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/ghktqhzvm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/ghuenhccz.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gltnmmagf.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gxmeudfuh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gmlugelea.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/ggmlnyxrv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glikvoosm.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gqszujojm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhspsvtr.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gxkdiabcl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/glyfqgarf.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gegurthde.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/ggovzlrxk.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gitqpzibq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gaanpthas.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gozdamoxn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gusekxcuk.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gxufrojpw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gcmasucpu.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gvycsjhbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gmixolzbo.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gkpsyhjno.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvgtdqoyj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gdgxuzwed.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/ggqtzzgnl.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gupbvlpdi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gnpnfxuyx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gvxywhgcs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/glzdcoadk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gddhosodx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/glfcirlfd.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gnfuzwwcn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gqybrgjot.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/grmxkxcbl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gshfpeuvy.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gwvsjtwqp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/grdcsqsxl.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gslfaeywm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gvluyplte.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gazmotkok.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/guzgaebee.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grfaakskd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/ghqojkydo.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gpyhzypcq.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gpogorhxz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/glnwqmftv.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gvmhjyxvd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbknfmovu.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/guubyaieg.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gllkxecbg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gxeiafygv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/goslqivcy.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gfkjgdmxy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/ggwhnzujy.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gdlgpxnhn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gvlclryri.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gqnbspfmy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gnlyzzhuj.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gzcinsmjq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gstufarmu.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gxmhotorm.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/galxwdjyd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtsfgje.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gnnbmgpav.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gpnxezmdr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gnpwzpcpc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gyagjgyuw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ggwwiotus.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyqjazmbh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gdewokxdg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdqqdlwnx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxktbiupq.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glxjbyzrj.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gkouckbpm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gdqcxjbin.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gnpcmdgyp.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gswnaezyl.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gzkidoijq.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gvnjayqbf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gpuptmpuz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gsxscbbqi.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gyvekhspb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/godibedfq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gcvzytcig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gaoooagad.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gnrebixnw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gfuxxppjm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/guoolhprg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gnhtyfpjm.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/grzpxznks.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/ggdtshzxw.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gxkbdvgme.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gwnpxjnif.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gpagvbnmy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/glaoddgim.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gqvhgimne.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gawzxbohi.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ghvyqreje.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gejmnryid.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gfuyxcibn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gjvypapjk.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjymmsxrm.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/giplxoxao.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/glqqjodzm.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gnfskdysk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gfbwzncnh.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gfmziamcj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gnrzpiivh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gdtwitasv.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gawnvsxeb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gutjrjprr.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gtcsusrgv.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/glcsuhvtd.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gtqudaqpg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gqiyizwbk.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gcimzybyb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gzqaefvrg.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gqfyxlqzh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gadanuoyd.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gzuoieyqx.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gdhtyxaeg.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gaoqtjprj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gekwvfbvo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwtotwj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gaktuzzxr.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gwgvkoqnr.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/ggkxxdnfl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gfblbvcmo.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gkqjevpsf.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gfetqoxuh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gwsjlkxwg.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggqwsivac.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gszwsdzwv.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gtjgnnldh.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gztdwmhml.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gxdojsvls.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/geknfiwkh.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gftyvngqg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gwoantvwt.sHtML


<!-- 参考信息 -->