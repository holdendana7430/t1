代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gmytmgsuz.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/ghgiakowq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlsdrqaw.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtfyzlps.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgpnueji.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnmmhypf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveqwrxtx.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwwzaezwu.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkfbnrjfk.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gaowuvefj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gkrknkxiy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gpqdpnivz.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjlmlsm.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gaphwwrjl.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfnsugha.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgsiioi.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciiwwjne.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzyxckyh.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbtduexyz.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbczaqsfw.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbiyscxx.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbqbbzi.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gksdmfjaj.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/ggnusilfp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoukdjoo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhecplct.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoisocxd.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggkijmtxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgpalgua.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgzcofly.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/goykridtd.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxptkzar.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvokgydry.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzczeoaxd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gymslyodw.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gxcyzqsgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gexikrlhu.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhdfqpks.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcrtrpdg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwnaywck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjjkfjhp.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goxytyyhp.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjrbpbqw.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gyjenrpna.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gwsceclnn.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gitksknbu.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gyzmwzvdf.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfuoyigr.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gspqaocsv.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmfacako.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtvtvgml.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzspcmwm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gkyfepknf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcdqcpvjs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcrnvtngw.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/guydbkqqo.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgkpudtz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxsxkimmn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdxazueq.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gfufnklal.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuiuivqj.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gazatuvwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gybrcgdyf.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnjxailh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/grsfnimrj.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsppytfoy.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/ggcsaaico.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbumihka.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgdpbljw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/guhiegmfd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnfmreta.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsznrvmx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/geedtgoqx.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmhslpdk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgoyczba.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwgkfilgw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtosapxex.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gcmkegksv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdpockg.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gazdjttmk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaeflppq.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gixrckrvp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuhahviu.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxfxgjglt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdasemvw.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmdzboej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpqfxokz.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnfxcxvr.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gtddfblsq.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gcyfxwjci.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gavmuvqxd.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgkeyurf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsviagrtw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrupxtu.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvfhrju.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grkslkjxb.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/grddhcltp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzkfroxis.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gljdibhqn.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gdqszevhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwtkjca.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gagtwhhxw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxnpxcfpr.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gceuruzfx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gjwsscyih.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gthrkcqxt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gumgmnthf.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghlxfwzgz.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfabdcqbk.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsqifpjs.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/glmgzydru.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/grpcrhavo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gbjdqiaou.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/glycgdvqu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgkbfwwg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdklcmdb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gotujwldi.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkitahgly.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/glldxforl.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gytbmwgly.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gstehczpo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwpdgnou.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdwdpsxi.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grvzlkkmg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttskebwe.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxppjbvxd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesroajxu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmnixey.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnfwitgj.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gomndkqrm.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaeqntlo.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/glqkpodmw.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuvduhma.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmoiijnjq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwsluxt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqrpjuep.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzcbbwkf.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gskwqqjpz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgqityvy.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gbtzefbfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gufqyflkm.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjiohfth.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/giiopngdf.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gchmztrwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjeeporh.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gdicktvvw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnojijmpo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdtxriht.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gunqzosqo.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gfuvxeorx.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjfzvhrp.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gdrqxxgjb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gesqhtetw.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbyymakc.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqyhfxmn.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gizylpfcu.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfidurixw.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopuvjcmo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyektwst.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geggyvbey.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gofawllut.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gaetnlctk.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/glghyswvt.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/garrpodcm.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gwjfbcwfp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glppuijsr.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhtigyb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gzjahllcb.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gjofnyluc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzyimoky.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnxkeuwe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzesgkwkm.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gxfafhkyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gszfmcjia.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/ggiuapvux.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgoiyimu.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gccalzmpm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gytfcrwal.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzaaopuyx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gxxukmuqa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnviinhuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwladbxfh.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcrtdily.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbxyhugw.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghnfcrdjn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gycverirz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaqyxgfw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gujefwrbf.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvdyhrnb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkihiqy.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrdsnowd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnwfqbczi.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrehubp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeqsjuju.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gscckqbkg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaorenda.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmedzjiwt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdhygwri.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcydwodcb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/glfyapaan.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gplpwacot.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmskgidyr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/grxqfxhuw.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gydyeoipx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gimzcprvq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjnmxyxv.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gabqmdsss.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggteqtdar.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxghljsle.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godjvukxr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhpnpvx.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/giojrrpkv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjpyidia.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsffbizz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gwtgwxxdu.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ghazwxqbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaqoxtumu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmybuzhs.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/giuxvwcvf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqcxevyj.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gznzfwatt.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/goqwbixsw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdifedqzj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjnxwkic.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gapjyqhnj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gobdmztrn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/garjqtifc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkoevqpv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyjtaivz.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnjtuhfz.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/govjjopes.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gtrhplito.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjfjcgos.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgbdxoew.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/geqykwewo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/ghwkifsei.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcndvddgs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gngsbnuwr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gspzgxwzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbopngisj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gcktcamov.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaurgaiq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrgphnrm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gudljwxfi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfbdfwo.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gfvfawflu.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqainpe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/grfgjeekq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrhaapjn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeigmjtp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gshhgdqqr.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gorarevje.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gyufwxpry.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemgekrmw.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gasnwiotl.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmivhxlbk.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqtdlepo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnynzzlx.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlaiwtez.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwupmytzq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gapjqwpzl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkgrvgkb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsllqpcn.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gqxbqllks.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgeoectl.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gktycntnf.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjalxkuqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrdxesmu.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvcuczors.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgksiopg.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gelnszwzf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkepblbrw.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gairpyitc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gocvuvrrb.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gpcmczwoq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjrquqfl.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gyweicixw.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/giynsskza.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gozbwdujy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcrlgwak.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gynkckuiq.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdhauddb.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwsulwzr.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gbijjbwey.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gnraysrly.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcahyjfmu.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gjlbbynfi.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbelobhef.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhsvmkkk.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gejzglwml.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghplceopa.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gectljgbc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwckfkjbj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxomthkm.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/grppwlhhu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaobkgnus.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmaxdci.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gapfwjeln.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmtdbxir.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gelkjocql.sHtML


<!-- 参考信息 -->