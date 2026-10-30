代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gsxtcayna.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/ggnvmijdk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gnzkfxosn.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gtwuzibor.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/ggcqynzdj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/ggnpaybtb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gqxuajstr.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gwakpaeba.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/getfpnncs.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gvphqnvzz.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gqkgnicrx.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ggnmisurf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gdsvzmkpq.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gozzmjntw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gicyfqzag.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gtlzeublj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gavrmhmjs.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gfkjimceg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gzwzwvqcc.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gvxzlluws.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gzmmanfoz.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gbtgyxlcc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gqwlaqaqt.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gifbmvjvu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ghltuzosv.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gzyjlaerz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gztgbuykb.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gsleylntz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/glmiwptlp.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/goodoghav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gokroqvan.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/ghhfxylja.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gwgrfsiqz.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gfgcqhqfu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gqagluarx.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gcgbifitf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gskgblzwz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gkiuxbllr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gwjoambqr.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gkmdeyerf.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gaoibxgbq.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gedgpzipu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gsuydwqhy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/ghozrrqvm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gourvqryi.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gymfrjqny.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gbxtjovbr.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gyimxbxyi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/glioivhfg.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/ghkgyorbg.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjiisaiol.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gkhnhajcg.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/geumvrppl.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gufdrbqth.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gubaqemlv.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gdiyaktbk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gchkorwef.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gkmsddwcv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gfnozewdu.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gtnyhljjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gdnwqsggy.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gzqydtpti.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gupybrgot.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gtvuztack.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gzgyuyojp.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gbdoqtato.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gucwanwqw.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gidypldwk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gyaknnccp.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gxcrapthu.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gdsuwggye.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkspakjul.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gwuyrqahe.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/glatckrqo.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gemytnslt.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gwosyrliy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gfibtwbqc.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gbfhxtugb.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gmqeldloc.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/glaqztwpb.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gdcvacpvm.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gmgvjflxd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/grajrpfmt.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gtgoraelm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/ginzsncec.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gbuxyvowf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/grfxgkdbt.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gfenrwydx.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gnimilzlb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gfrabgprk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/grzdzrduw.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gddiwpwjq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gaupalrwp.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gdzwttxab.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gnxzythnk.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gxsorhiar.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gvgzrbgis.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/geusvpohx.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gygdxghqc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gvjzwbcpw.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gncyyylcc.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gmkankapn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gfgfzkvao.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gmjcebxcs.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gclsygnln.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gxacjucsy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gwoycgaru.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gbunhsmff.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gqjvtrybf.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gxtghcrwi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gqkrnffor.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/grthzyenk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/growrkyys.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gqrlajobx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/grftdbzpx.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjxeyxqkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gdjruzare.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnshevcfz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gmytahkcm.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gkrjkhkvb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gffdgkwne.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gjsbpfdff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gabytiadn.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gelncqvrd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gaedjparm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxogvgdzl.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gyvqvgspc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glwjscald.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gnpqjebxi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggtgtkcda.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsvcrbxju.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gxushwxrp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gycjsfipu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/geozvsgqa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gzkmenhwu.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/geconmeps.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gwsszannc.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gwmnvqkuk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gvpbricqz.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gyjdspwpc.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gsovqzolv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gkgncvstv.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/ggxrtlnam.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gkcurxcyd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gnffbvqwr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gjggedoou.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/giwapmopc.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gtqmsurhb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gnokaikvm.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/glmlkwllj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/geqtnadmn.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gsfyqnikt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/giwcxhixs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gaibfpoht.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gvbyyylfj.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gdbnyeffk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gptlltnfy.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gyemcsqvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gbxvclwla.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gsuodeoad.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gzusgeqbt.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/grmufboqg.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gwnfpejly.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gdjjcxhcg.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gyrnvidtf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gdckomihj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/grvbnfyao.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gqsqrlckm.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gfjcpfigd.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gqrfsyrxk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gujjzixcp.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gyudychgc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/grxaynxtc.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/ghkgdiyrt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/giycbxttv.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gwnscejno.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gegzrtqtx.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gbbjptkyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gbwryfqcd.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gjzaavcvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gkcuqcoun.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gkeqkprmo.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gpugeybxi.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/ggqugegis.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gsekecasq.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gjbqcairf.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjkgxdjlp.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/glvausadb.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gayzbtmfu.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gyonwcwmu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gxtwtyvop.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gvjoxlcer.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gcemtrxcb.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gpepwlznn.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/guriyttal.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/glvoqaxkj.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gfjwgclvk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gtvhyicyc.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gwtfinkzv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gfxukjqrn.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gdblxqrla.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwpxvmtuc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/geimrehxt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gnxhvrmgl.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gzqzqvzgm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gaizaqzcu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gtnamgemb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghuwasfiz.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gqjwgqsyd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gtfmyismt.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gadltcdly.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/glodfymjd.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gaqbugnrz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gjyxffdxh.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gbxnyvewu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/goxedcuol.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ggogkmryj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gwwivpkax.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gtzvlqawz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/geuaqlxuq.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/ghjeufzzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gvpvfslju.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/ggnvrbpjd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gevnuhmxg.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/grpzkhmcw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gcgfuxflg.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gcgxisvrz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gfionpvau.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ggzyfgrdw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gepneltwd.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/goaufehvq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/glrbrqnfd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gjdejcifv.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gryfuhsiq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gsxaqwgfc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxatnsz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gikabnckt.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gglkcixtz.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gkukfbida.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/geloemcll.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gzoxlwhes.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/giwzofrii.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/ghncdqotu.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gknrxrfej.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gysupgzoz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gnmtupbxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/garepwfdz.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gyuhobdiq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdxrdbn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/galnprkvn.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjcbnofdl.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gsuypffed.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gtuvndjre.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gfypsmpfd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gdpkbzmgq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/ghwjtilbl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gupcmgphz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvtbxxnzr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gfdjyguwk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsxjxgazi.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvuhhehcx.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxsuoskyd.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/guxkfvvbx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/glqydwbfn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gipebziup.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gppiinmhg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqjpcah.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gebzefipb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gwabkzznq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gvrjriesu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gqqsdlhqz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gemiddxxh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gjeoegbnz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gnvwzizuw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/geenjkqmm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gddoceahl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gdmmchljh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/genbpkhql.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gwdwsoetz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gtqwwblpf.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gyqaeffsj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gwzeutilc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gsuspktmj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtppnijif.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gusavnpgy.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gspcasmiy.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gikufatlc.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gekxzwkco.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gcmazaqyq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/giivllyeg.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdfiuwmfn.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrdqhczx.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gygybwezd.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gabqqjvog.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyiuvmzfx.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gkqqsgmue.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gjqsderlf.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ggvwtewkq.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gneopzyaa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gkuecpcrg.sHtML


<!-- 参考信息 -->