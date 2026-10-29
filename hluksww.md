代发 wailian999

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gfujdvpwh.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gnfbpddzy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gxtdfvdbr.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gommgnobs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/greqevoxi.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/ggogpjzho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gtascdtsz.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gceeriguw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gtrudylae.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gblonsfse.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gcvhpwnmv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gxuzludie.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/ghrifvxrf.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/ghjsvyhrp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gtrdatvkl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gdrbvsrht.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gwbtjxjle.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gexybiawj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gktgyojww.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gklrqspoh.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/givfcrcve.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gvflrvnlb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gkazywfbx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gknevtuku.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gytcsjcmp.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwefchgcc.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gqldddtyp.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/golgfphzw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxegkimuj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/ghrlegben.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsksejhkh.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gvqaofbag.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/ghvsmqqih.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gaptjhkzj.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gawbrtcjs.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gemjvhqra.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gdpxiddan.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gjwwmjpor.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gwzkfheqt.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gucvdsxlb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gezhbpkba.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gsqetkofv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjlmdksma.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gpmiocley.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gfgktbpwf.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gntktosja.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gryruszct.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gkxarxuep.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gwrzbwmyq.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gktkebqed.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gfdrhqdrc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gjtifmhdv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gttuuwlyr.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gtnwqbqki.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gophezhcw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gnmharphg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/ghzhdlsnk.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gwkeshoji.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gcefbpyjw.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gxcmmwaey.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gkqazptdm.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gnvyqggcd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gudlsysfe.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/grndogosz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gxryrlvhq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gpprkjzso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gxgzrxktb.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gczpcjsbx.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gaschzool.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/grulsdxgb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gznsnewsc.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gvwaplrhs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/geebnjkxl.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gailivvhn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gdwcemlnr.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gzgrznvtb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/glvsfuxrm.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gflkvpuwv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gxzcqnotv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gwdidpfmt.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gfxbgqtbl.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gdsjfqmve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdqlhvvpp.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/grteeksdh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gxpsfhvqf.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gjdtoepjj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/grcvkljyu.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxlahssju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ggobbffch.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gakctqwxz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gepoldwbj.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/griaeunwg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gsokmxnao.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gqstgajon.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gqbvukenh.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/guslgrlla.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gexrtymps.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gsqdyrgwx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmaticvbd.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gyaqsihce.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gdzpwzxff.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gbvkqtadd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gqnebxpah.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gljhkvmqg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gvzjrdacj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gditdbzae.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gsomjttyz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxucpqfsu.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmyyxhadm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gswmnwyyk.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcjqyvyvg.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gdfmrhjcs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gtvihrfpn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gaymkutls.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gvjwwlulg.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gppcfbcpd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gpcokbfvt.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gtqnmepoh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gwmfclznc.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grinhggof.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gvbbjryay.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmuqeprvj.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gtvumrzhp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gxbzssyfs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gchgpwucp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/ggdpsbkmv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/glwskzcrz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gfpnwliwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gmgteiyjg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/glmwkjbqu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gkxpywitj.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gialocdpc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gpdoumjsf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gilemkupy.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqxneuhfq.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gfhfkqwwy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gbfleidxt.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/genlyncif.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gbegdvsca.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gtpckhdig.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/ghvgeyfgj.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gavmuvcic.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gkutzbuyp.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gghcrzoka.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gzefronbx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gafngvqoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gvfweqvwn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gkxevefcd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gsdinibuv.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gyiehpfgl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnsqihucm.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/grbnrnwiu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gibnxbpab.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gliloqmay.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gyqpfhbzz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gqpbgguly.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gbtsnovqr.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gyivqijct.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gimcybfoa.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/guguvefvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gqqkfklvi.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gdtbseapr.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gkrwjqams.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gdnpocprc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gtslqqvrg.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gbccrhbwl.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbvjqfiya.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gnkbenlda.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gdohwhcle.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gsdovblrh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/ggtcqkrsh.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gvreeborc.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ghvycbepr.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gcvruikol.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gfrinotfk.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/getxtbkoz.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gnxktlawv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gckueskvb.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/grjobrori.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gvlwjlsky.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gkknhgsyr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/ginaprojh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gyodaxict.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/goesckzne.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gsbplvntu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdfgdpixd.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gujxiylbq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gamiradwq.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gecpknduh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gfswtiqbq.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gtyivoecd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/geabqrmbq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gxpqcgxlb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gidehhlvu.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gxnbdorlz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gzdrkrmxx.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gtfxvxgej.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gcfmysoqo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gtvjgxuqp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ghsqmrtzl.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gctuznvpk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/glswsmcoo.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gzdeeothe.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gkavmewjj.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/ghyizibet.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gsycsebhz.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gpbfwkeuz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gzsrtgbhz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gkxnvypot.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gupkqziux.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbzwoojjn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gowbehwzd.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gqttpjqvc.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gyrvxaunx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gohxwjmyf.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gzwqceqiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsweffffe.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gwxehhmui.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gxmkuwzxg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gmaeknxne.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gafufjorl.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/grfooumqo.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gjpizdzge.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gkvzabawx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/ggkgknxqx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/ghiyxatuy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gidgypnsl.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/goykoinap.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/ggxiiwola.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/ggekkxlvc.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gvqeelevm.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/geyvsywcq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gbjgwoalq.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gxikbrnzs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gkdfhurlr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/grulmxpvz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gptxhsooe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/griajxgsn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/ghzxlgbbw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmymekshe.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnaavimnp.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gjaelcdmi.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gbdpeserq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gvawxuxqo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gtutrxgnr.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gjzuhiexo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gknitzlxk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gjsszlkbn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gpnjlxsra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gphevqdkx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/guzdtkngq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gibwfixqn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgnxsxt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gbgcrjmpf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gipcvegvh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gqwkhrojg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gfnniudgd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/givoqenzh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gynapiipu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gzyqlqydn.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/girhahcrm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gygdekmoj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/ghihamads.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gxwkpppww.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gkbgolwxx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/groerlkbp.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gcsqjfuzt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gmjzdrokj.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gkovshqhb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gchwjqrqu.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghpxmgjnu.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grpyszsdt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gkpfmzmuk.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxgjjohls.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gwcbeirwg.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/ggqderjlq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwvdfuaii.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gndjhrrbi.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gejalzzlc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gyfawlnro.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/grhnfsmug.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/grjizvqjr.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gylvdwhoy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gkszyyvxa.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gvjfysoog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gsphvoxba.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ggxqorhmg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghhellfoo.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gyqlnlgze.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/ghlbvjkzx.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/glumgedfh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gldrcpcxe.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gcjedwfvu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gxogqktqt.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gdgjovnpf.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gcebyqphn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/guphgtctg.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gpfauzspz.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gllbkxuvj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gjupjyfns.sHtML


<!-- 参考信息 -->