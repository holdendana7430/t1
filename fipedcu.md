代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbwshihp.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtyuzdwb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveelrwek.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gghhsfjdc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyogoizd.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gjlokscpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxnhgjh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvzjwkwh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/genlywrkn.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevuirbvo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gotwavsks.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyeazsil.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gvrpkmlpr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisniumzz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjsbarkj.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gorwdflts.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gplylokut.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkgomvmp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwjuujooo.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gvomgwnuf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddyowjcs.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gatsgpota.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/givhgsapf.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gaelnhest.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gwjlkoxqt.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gkbnbpacj.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyphayic.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gieoaxwad.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gowgsxhht.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqwwhnehz.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoqufnbq.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gidpvmsmh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrlxcyy.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzkkpwsvs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gnrqnbdks.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnvhdbyc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbywlniqp.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgvddcfo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqshqgzj.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gizxcxmgl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gzmyuyghc.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwauyfyqa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdsngyyjy.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakllscna.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/guikfwnhg.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gucuixkge.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpjgwmomu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gainwdzjl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggdslievs.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gadwbtkpc.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtohxflqu.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gprbknoww.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gybftmtqb.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gqgjksgrx.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gqzsedkqg.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdkblwxm.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gklubbhoc.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/grqwklwkb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gskdgrfhc.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gdjpeqfoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gajbszaps.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gazotftpl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/glrqdhmgs.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyazvugox.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyctjpbuy.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdwtrepzo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdigsfmv.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gavipbgfn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasougttz.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/genxvunmc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/geaavyeul.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfzyewlt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxbjizia.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/glfkyozqe.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gzpawqzhq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giapbxotz.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gjiakwxni.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyhrrroe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gguzzafbj.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/grgiovofl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gwszilote.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gomstrjva.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmcspgat.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwfxeosd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxkpfqqd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrjfztrd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwxngaoi.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhzdnpvh.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gouwqqneg.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gtqfhrxtg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gujittfmc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqhsztdqo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gncgqmqxp.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gikzjpwrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gtstlmhln.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gkrxkvkof.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfuvkjaa.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzxvxymy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gayutctqd.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gnycfgkyq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwimhsfou.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gquspcohd.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gotplehnr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaotnellg.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcomekb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzvykqa.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggxazymit.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gjvbcwixy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfijaztwz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuesystj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gohzcmalz.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gseoilubn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdgpzsok.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbfplzvo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxttcidd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gelulivxr.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnyoqkuc.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grwrxtyug.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gkjylexnt.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcccotrua.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxisqvm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gwuomxjwd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylbjoceg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gjacfdjhz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmofvexyn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gutascxel.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuyakevi.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaktxyumr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhuuwrxc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzolpsw.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbubtja.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpzcxplfx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqcwqbni.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grguelhac.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvrfhudo.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfvwjefh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gommclopr.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdshsdfy.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gdxavxtht.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gvprzlhre.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuvqeqjh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gggyiegwn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqjmdxdw.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfmjkwgo.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujljipho.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghbpoqbfj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/grzkaehpc.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlryqlqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkidkkzrj.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gwnrnjogu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/giysmoylt.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcjrgkrd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gajqublsy.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjaodtxe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gbkhnkjcs.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaortrri.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhiiqmae.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grfidzryn.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gskskxmdp.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfhhihep.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhghygbs.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjmpivou.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqebfnwhq.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqvxosfws.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjmbfekb.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbkqlxkb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumebpzk.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gymesiemd.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzddfqxwi.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrqcznau.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ghnbhsrus.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgcecmfs.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwdwbgeb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjqlheni.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuonjznn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggijkbkvb.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gsnsyspwz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzosetejv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrbfebqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggprupqgv.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghplfggfw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gplszxnsq.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gvxusuojp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggnbkcbyu.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuobjnsr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gopqqored.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtqlnbyb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzekzktla.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gygsobqvg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gauysrqpa.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvndeetr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvmalejy.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gclvbouje.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/goyzbrcks.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfxucqqnu.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gawhbmzvv.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gzipxnhvl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gijpuqlsn.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gchweflnx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcrcwaode.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmmhoqsl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcolsccpb.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrjzzpyg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gclqtexwu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgeydlvv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gztyemwdm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gezmtqazh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gtfitawku.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/galhvdedo.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhxnyjrr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gezkzaaoo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gswgdrsnd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvrlieru.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoowyesy.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpotkuee.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gjtjjyyeh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/grrdbfplg.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/giffvopsa.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbiweyhv.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmbkhdnk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfgmivvx.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/giwrunjxd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfiiipmh.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gofzcailb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/griqykgnv.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbidxqgsf.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gkyljdeje.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/giqbkqwuy.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gcfqodrro.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gscnrkblt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gcmgdchdl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/griaoleoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/guksqmxcl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gftlruymc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gomqlpaxk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gizkgvrpj.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gltkbwnhp.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfqrqblc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohhwtnwp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjwoasuk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoqmvnlp.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjetefjwg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gapzpngng.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gsbzjsqij.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqhlkffue.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gekobyiot.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/giasxqhpp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/garhmbqwk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjtmkbtf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilcrxmvr.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gdbqoxxxn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/geaqjvryj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxitcxddy.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfsxsojc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gosjnvwpb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgrwltaz.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhmkhyo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbrukngq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrgygurf.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijgqkzln.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gjgbdjjgp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuafqapd.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/grkdklrpu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeuvjuwo.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/guhsosnjy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gigesgkjl.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsfyqwqqv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gocujhmnp.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggqsczhjl.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glreefzmi.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/glzpufegk.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxhswllw.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsuzujqn.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmfdnxbbp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbghqtey.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnsvoiz.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxslqirl.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggejoelqe.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/geemyoevg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnqfpvzse.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzwhepxox.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkulholmf.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnsjbds.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwyvbjux.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gbukwztie.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/glegumrus.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/ghijphhtq.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gtanvnido.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnxeggoi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiekgzhi.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/guhlreijy.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gghzxhhti.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrlmfjoh.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnwlozaa.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gxiqdmtbg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gzqzwgdxp.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjfrlwaom.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqjkitbt.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbppxxiju.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfjyyuzm.sHtML


<!-- 参考信息 -->