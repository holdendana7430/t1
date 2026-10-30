代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/goqqwyihm.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gnwukifwm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrjgjfdj.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzvojgmk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnlozaeo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtvpimcfy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gogsqjjwq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gubqllxcn.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/grvlknccj.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gwdenbzpb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxbcltkp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmorlptf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvbgwkcg.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcymcmdz.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkmvltfx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girbcmbkc.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gczerfpxd.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gtodggiaa.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhkpvpje.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzajostwq.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrunshxu.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gzhadfkny.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ggzbrvpcr.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukrbvzwa.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuvxygks.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gvhxtxjyk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grepemuhn.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guyhgnujq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghrioxfoz.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfqoair.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcglbwqpl.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gldiigvlr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/grcgdldzq.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gdhnlamkw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwdzfxvi.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmhnngnkl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gdflxmczs.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjraoxf.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxlltnh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavswujyh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmyfodmfl.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gayrhttdm.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlvevjzi.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gntclmfmr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gseahiflo.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gisyspoyl.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gtzenoxcg.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gonijfmcd.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gahzqjlro.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gshvbuyfo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gywwhzshf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxggttrpu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/glwdhewvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gvrdkwsjg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grxpflpok.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gqidfuwfr.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gogfegnkv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbymlssl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gktuqyasm.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkjurpfz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpsdzxxh.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gnldkobek.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnqmytfpk.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxymsftzr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gynhjyokt.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gehsemhur.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydtknyxd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gbkbhxnub.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/ggehdtbzs.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gvzesmjqm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goxotvjxq.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gwomadtcb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtnnmwow.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/grhmlahvn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gpouzzlvm.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjuforib.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxseouhv.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvrhmauu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbcwwtja.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzsuzhtmv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauerhmme.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozzvccuc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbztyodo.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcnpkzzqq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gefgsjwjs.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwktixxt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gbntcjocq.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvrzojvi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldpokbyi.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gfchlxdno.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtoeeqemk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfstmxmz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gywncpshh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkdzupzx.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gdseaqctn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduizorur.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkuqtnjaq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvhfdeyym.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqwjwwnls.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjggwqxft.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzikywsaw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzqvswvs.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gchangxfj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmulkxsfq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsivxvgks.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/goohcejkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdywwewqw.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpmilsele.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyupuhscz.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gycxjapbh.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gmbzghxzk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmfbtnh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/goyqgaxla.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gzswueiom.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gxsskbhss.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gicfghlzm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ggjbgtdvx.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gnintidxf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzkgweqh.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glpmhkkqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gcxbazkzr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/glugxhuec.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehtygic.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gywawnwww.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxibeeum.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqmmhumy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrhvnsiw.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/geonbwtuo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gygtbhewr.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxojgmqbz.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbtfeibz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlqzhijo.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghuypfrda.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyjybyenj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gynmqgmrs.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwswohmvk.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaykefqjd.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcwuyyfo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaqpczxj.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvctlstm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqljrdmiz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacvslepq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjzdwutl.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gpltybnei.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gdnyighpf.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebbtzqq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjghqeonz.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gniicgxii.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gslvpexmn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gewcfzzdq.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gdgritcez.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhhiwvkw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqpeujvm.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjnkybxw.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvapybra.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdklwarq.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhfvgyfm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwmrkecx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gnbolnrie.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfnocowt.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoefjfia.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gleckdcfx.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbmbukge.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gglszubdh.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/geodgxrlh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gausrsmkc.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gogntihpp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gslxrbbhb.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzncjqlm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gculzwfjb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ghrapfvra.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkacppsaa.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gctfiyhhh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvcidezq.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/goajatjps.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxhwqnzh.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gihuoertz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gheeqlqaq.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/guoknnmri.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/glarfektl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmdkecly.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlbyxfor.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/garqmnoem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlswenym.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmncyedz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzomsqjb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gftbehocm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gjuenwlqa.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqqvezyz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyhcfomx.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsgdutro.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gccwaufcy.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcttnxjrv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfxqbkai.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gmjussylu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmbewpeh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyaeblbwv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gypsujkdc.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnasgfvdd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gmqblyxnu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxealcqgd.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdegmlqhc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnibteqnb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaciinbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/glmpxdiop.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guukrpdvo.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwygmdjyr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gomqdedxg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glidiekov.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiqvczmd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gihujnxsk.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdfgzthuf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnswqks.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gxfiqaahq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/glfbyxris.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gjvtldrdk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gldviqmjo.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gjttpejjg.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/geecxnoef.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/grrsgkxon.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcqoxdis.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfpiejpx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gazmmasbx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gusatjqpm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgbbxfza.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzhruveo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gamrrshmj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjazuzeb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjoueitto.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gezrmnpdr.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqxcnqp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gxvqowtjm.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/girjuuein.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbzsypkr.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/guxhgydlg.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/ghutmqrzt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzctrrqah.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gjqulgets.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/glvuzsfnm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gagxtagvi.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkpfbdmfk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnioufhlf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gjrssdzzw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gomprrqri.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gozqaruvj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcbhlyhs.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjhhvpgu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfozgbtfh.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gjgsosfjw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gxlffjugc.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gsusehrsn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwqlznaau.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glstevmma.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggwtmicpp.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glvcmlzvu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfvbcrea.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhziwuyn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/geidnoowy.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdpltbqsz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjfedbqk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvrcakgo.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grjfiefyz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgmctack.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gmqcrizlu.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqcgdowvi.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gknlqgbna.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gpdoxesmm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gemfzxhuh.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gyvupnlhv.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbkiyeuk.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gliujvczr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaavcbnf.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxefyprk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxcmrxiu.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gilubghgf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmlaqxgf.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gktbngzjg.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqgwirwc.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gipokvlus.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gmzckfwvl.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyzvqahh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gavjnwlyv.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gsczrwksv.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjedrhxh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gkplmqdsr.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gvzdbqnsd.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvbikoly.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbefjwdz.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfjyrpuv.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gctgqcqmv.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvidbfpni.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcvlvios.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gmwoxeqae.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdautdbyn.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gdugayxmt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/ghfnuaxnw.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdusnnqev.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopnnpnas.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblnxwsci.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjrqpcb.sHtML


<!-- 参考信息 -->