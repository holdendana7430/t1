代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/grszkktla.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gwteradtu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gcbxunrfr.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/galqpvdcb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gzmscplki.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gruennreb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/ghaxrqzgv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gpdvnntsc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gkprmbgqh.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gqrffyypv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/ghvmbfwkl.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gkooccrkf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gdjwfpnaw.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gbrjdbxsu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/ggvmydqmw.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gzbkbezkz.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/ghqeytmns.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gahcgkcgh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gejuazwia.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gocejmscw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gwnoadoqq.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gggzclerb.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gpourbcec.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gkkengjzj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuqoosk.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/grmxcoqui.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gfdpnimvh.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gtsdyjhkq.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gcvgbnusc.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gxwdrmkqf.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gvconfegz.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gjphuslxd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gjaovkpmx.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gwzlmzcru.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gutjmgsvh.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gulmibpcg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gcjcglshw.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ghpbkdltl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gktpkdgfc.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gfswlsrpc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gvzobrnpn.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gnvmhteff.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gppchsvjm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gstyukjhe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/grkycqzuz.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gtsqpxpsk.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gsotxkpni.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/glpntwljm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gkrwqadop.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gfkqhkafx.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gmgwnywpl.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjckltgrt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gltmesyma.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/glgpmdkha.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gclzwcwoi.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gedyudilx.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gwpctfjhg.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gwdwxkeir.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/glvuolgxz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxywhjhrt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gzwavfggf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gphrylsxx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gdvfmalrf.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/ghisusbnp.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gwhjvrxqy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gndlsbjbu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gdqjvchil.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gzozukfrh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gbxikqdmw.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gcbhntaxc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/goorvfool.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gqrtquhhr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/geendxoap.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gfvfmmceu.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gufuoaszm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gzkpqdrdk.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gvnjrtvxr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gtdywtaan.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwrzpzikj.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/ghyuwrosf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gbcxpdhyk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gmzjbdbgm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gaurswqel.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwwdsfvjs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gfzumrmot.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gkzylyumu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gtpflzsrb.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gspwqrzeg.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gwkgmkgot.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gixiykrsc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gboomtgpj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gtuudrrnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gjxigciew.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ggiujizey.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/getsubqdf.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/glzfuvujj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgbgxac.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gcrpjuuyy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gpjaitxol.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gftqrngtj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gztnpdzxf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gmvnchjnc.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gqcwtawnm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnypmzvmr.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gmivccbnb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gypxyssrh.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtpeoliem.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gkdmlaeah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gtjvayswb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/geaywrdsf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gqvskkecg.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/ggysvumby.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gccaumpet.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ggrsnvhnn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/ghuzmwbjr.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gyimhexon.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/glkzoyshd.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gazsatpwh.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gllpmjaaw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/grmdosmwu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gdjnvlvrp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gboardrol.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ghhidlimu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gpoxvjuht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gnivlqtag.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gxvxmytlv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvqlpsabv.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gktdwanck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gnnulmrxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gpywoorra.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvhzllzib.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gosnskgig.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjwdeoord.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gnizwpzmr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gaznpning.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gleakwnwv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gvpsjayqp.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gvjnprfqw.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gdseyvtjs.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gbhfyzidu.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gbyompngb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxlaqrjzb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/grvmbgjyf.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/goppfziqi.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gttufyvmm.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gsaqfkxqn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gbyssjybr.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gmuaaljhk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ggfyeicaf.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gnfodccej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gpwnnnzxm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gcjsxcyfv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gaygvjwae.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/ggheqkdyt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gmkizlmsx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gpzufmgaq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gswmosvpy.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/ggtmureid.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gphhipqxu.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gwiifpbac.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gbdxqbbww.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gsltkitln.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmhofendh.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/grkxqnzlf.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gsunqmzlh.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/grmvvbgid.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gsdvlqbdk.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gtxgpnbnb.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gwyupvqmi.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gecxsrzla.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gtephjpnj.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxnekdayv.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gppewbklj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gnawfkxtv.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gbaixdowe.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gxbdkrfwp.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gztghqgkb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gzxdfzqfe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gmofiizcv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gpfagggrm.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gdgacxqnd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghzrryndo.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/ghpawalkf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gwhzfrlsd.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gexatmolx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gxysgsqxz.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gqtfahvma.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gfkpquxyl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gjnhfhhiy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gyglkcptc.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gtchpgykp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gyqwgqdwz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gvqybssya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gfixqdweu.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gxvipoego.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gqechpfwr.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gutqelwha.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gvxwxdxqd.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gewrzdoun.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/grczwnlys.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gkonrjegq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gxxaseavc.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gddybjzcf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gveloivam.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gocehynba.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gzrxivssv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ghxsktuyo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gakirhfon.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gqircqvgd.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/grunlebbk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gpgisrumj.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/ggefwkzlb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpcqicpmw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gimlkwlam.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gyovuvede.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gfgvyeipw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gcrnaktwl.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/geknyrveb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gizkcnant.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gbgayjmvw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghnvgpztc.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gowiftpzv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gzutidjxz.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpzpcxt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gpapiaqrh.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gvgzotksw.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdrhefimx.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gpjpxhjkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/ghtfiqfpf.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gneqdmwbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/grbdcwrzy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gkfprwahg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gxwbtdfiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gewdcbivv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gtinzksmi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdvdxpbrq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grbfmbhim.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdfuzjbwc.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gbhnxvqdz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/ghqhqpyra.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gtetbqswk.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gypgnfazw.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gzhpygprd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gbbwpsqug.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gysnuaipl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gimmcuohs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gxggiawmd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gmdcbjvvr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gmsfqbchv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/glcmbfsho.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gyhpgljsy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gzxfqrlyv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gnpzlemyj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gzlonyecb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gqcfycwrv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gavqecmwy.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/goinuhlms.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gpbakobpf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gaoyeaneg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gcnltsyzm.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gnefkdnxe.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gpnijwhfw.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gqabsekke.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gpqmplgpv.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gjjpuslbx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gdgouwcwd.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/glwraymya.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbaibytyg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gshthlghc.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gpeqhfldg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gfvbhsclr.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/glyshtdvf.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gnikdaigy.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/ghvoyxwzh.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/ghbsocmft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/giklttmmm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkhmrxcja.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gjxizbmfd.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gqxrzwaul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gajuqsmzt.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gbdpbqncb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gqeffglyx.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/guytscdfm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ghgoroqlz.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gygdrufpv.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gilyffslv.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gmlkmuwod.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gvdsklxzs.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gfxckopmk.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gworbwwvb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gvthmfiep.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/glnfzmybi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gjpzbwkib.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gzvnlubyx.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gzoxdfizt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gxcomyquk.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gglqbcgqc.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gyzvxbreg.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gwzxcdsbp.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gxglsvzhb.sHtML


<!-- 参考信息 -->