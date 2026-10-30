代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/ggjmpylej.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gagusqegy.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/giltlsran.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gsddnmmgn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gsxljasjk.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gvkthysij.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gorbrrfnn.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/ghrqhooup.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gcbxqbkig.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/glmcioisu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gebfiwqah.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gjmywmedf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gdzwzfyjj.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gpqowtfqw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gnkrhhhol.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gfjxiyblm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gdydttrrw.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gsrrscfoo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gigzcqjxp.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gvriwquiz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gmhhkaozg.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/godohxydz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gngfwnrmh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gwzczwoth.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/ggjbwhqqp.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gbdjgzvnm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gnoxadizq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gklzkbabh.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gkhyfdphp.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gtzqgqypw.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gtxhctplb.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gwydlkcas.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjwahhaek.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gmdvhdcqc.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/guevvitqd.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gzdmizafo.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gtumwuahu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gbwjtxsrc.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gkwrlegjb.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gxtqloszs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/ghtmnrpwz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gbpfxrbuv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/ggojacjay.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gayrnidpj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnwetquro.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gkjkkypey.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/grvnlzvqy.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gsciaxuta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/goccipgim.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gzppftozx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gjjhrzskr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ghmmblced.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmxdifrjd.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gjfjfxhch.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gpqbirxjx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gjmsloasu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gjqugzhsf.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gtroyoqii.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gncfmehcs.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/giyquuhku.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gabeipdkh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gqoxzjyos.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gdjzzlmkh.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gyxzpymfz.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gjwhmqsxi.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gayyyphjh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/glctsfogu.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjlnscyer.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gtlgafoos.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ghhzvwhjn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/goldjcmou.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gibouajvp.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/ggysquurh.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gmuxfnyoa.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gpfqfndna.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gjfjwlrlk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gwstaupbd.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ghwaccbyq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/goqanilpf.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gkcixbimw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gyxvbxfqx.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gwsbblwjn.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gjglxirsh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gmkzcqcuy.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gswohvmfd.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gcxxtrknk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/givxrbpsf.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gdhivhqal.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gqntpmmxx.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gkgpkarbt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gxyyvvrwj.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ggplhlexj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gryidmrhx.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gfttbxwav.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gtktvyojr.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gcslzrbgq.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gpsrecjto.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gdtgqokjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gtltuxuqe.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gyuedqphv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gxloprsqc.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gwqljnajo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ghnieplpe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gycatqgoj.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gahybperu.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gfpdohzve.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gzplexpdq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gdefznsbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/ggwmnroln.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gfcpitxqg.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/guxzlvjtb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilknmngh.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/getjtdwyh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxgdrfetq.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcdtniaor.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gaoxzrsvf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/ghejodefd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gimbhbuno.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gtjjaykwj.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gvvbsqlms.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gkekeqchw.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gwowckyuc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gkowrdyzk.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/grisypyfi.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gsotmrdwz.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/ggolfjjbg.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gsmmavknp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gftjeecaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/ghgvekxgr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gychbqijo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/geynmedqe.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gnjbcnrtg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gxlhwswct.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gdteanhxm.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gofdghloi.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gyudrgman.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gsctvvvxm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gtyzfacii.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/givoadndb.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gtspchzml.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gvxqkjcku.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gteoqoclc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/grucjhtsx.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvltdvowr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gmjfpiumt.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gossyptkj.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/geogdrawf.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/grnncutqq.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqkyomg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gkvzqfikf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gpohmtoqe.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gaggahysk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqdsfmns.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gvcbjrgbm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gcgphdnmf.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/ghwhchabe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gvdsbmlrn.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gzdqcvcmr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gfpqvlpzx.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gdggkubir.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gliqlekav.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gbeanqpzk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gulcwanys.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gabcveasv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gmprxpuwt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjwiwjzba.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gdlmqjqan.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gftkmqvcn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gfxxztwje.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gdfecceuj.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtiavtnuf.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/grqwxqkrd.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/ggwbeivnq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gwzpdxlrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gubtazmyi.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gjjxwvmok.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gltyuiste.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gjyrahztz.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/glbkhipcm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggsvyxeig.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/ggfvkugpw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtjhssddp.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gilrmrnmz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gtlmoimrf.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gzkyeeydy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gxgvoaxrr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gdvuocxas.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gcrhdfsjm.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gvhepdiuk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gncunecyw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/geumdfrzh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ggywawqxk.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gfoffispo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsknkqatf.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gijjguici.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/guamkervj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/ggcjccykk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gfvwcronc.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gfiqyhfkj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfflxnkht.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtiyiozjh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gbxizinur.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gwqcnunjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gylhrnjhe.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gdhuwwpiw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/ghxqxydqh.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gfqbvblsd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gkdyiwuef.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gyylkahlu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/ghmvxbjfs.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gklpbhqap.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/geuuiokov.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gezcjskkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gsokrdjyo.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbzdxddlv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gsesnqymq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/grkfvisyx.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gyaajcema.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gphzlpsmf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gwnhlaoha.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwuoiyicr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gbjuevukl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/grkpgjmui.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gzdarnlyv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gttmyyaym.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/ginjgbkwd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gkgwefyje.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gvdpywubm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gqqbyiqrq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gwojhqtpx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkporlcfe.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gsvoqaiiy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gloktkkyo.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gmuvesugl.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gvksrhdxh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gmwerapcy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gvwhrwtgn.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gjtyaupku.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gijhntcyq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gmdgeffbs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gtytftgxl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gobmnazxa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gonniprbe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/griqlucnr.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnbcjaijy.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/ghrmytukj.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gzlccrnbi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gikrwxclz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvltpdj.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/glukzmdnn.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gksgbztac.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gciezfczm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gudtvmfzu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gpfxmfjxm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gdohurdme.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjuwzgnnx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gkwukulzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gnceeghmz.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/giskpszto.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/geasdatsx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/ggsqywxvx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/grvxabhjr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/guzpulkwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gvdbifdsg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gnmxapgjv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gtqnxfvyn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gjdjxogbt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggpfofxhe.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gtdqzvrtn.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gufpjuyml.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gvcpdbasn.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/ggqdvjrgj.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/ggymcwniq.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gxlntwock.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gktuswdjs.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjodkmknq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gieuuvosc.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gxedkmegu.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/giufhlfta.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gepzurnkz.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gpwrjdcfc.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghxzsjiax.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gowmevuwe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gaggsfyfe.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gwwsufzge.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gyogmduao.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gqsyptqaf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gckchjoni.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/goltzmdag.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gbqrwefpm.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gpktcnoms.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gquemahmv.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gkerqgpjm.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gpatkhrus.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gnhzvlztk.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gudxjibbg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gtpknredy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gnywzfmho.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/giuuwtndl.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gmanpwxva.sHtML


<!-- 参考信息 -->