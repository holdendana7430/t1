代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gyibsdiot.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/giromcbfn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gzniuolnt.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmlfpmrcp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gjquxklzl.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gotsdutgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gbenubhzv.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gjucidvcs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/ggnecajqt.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gsqkdlydb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gistuzhjj.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gyyenudlc.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gvqnpdenr.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gcjkdabii.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gswdwclla.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gpksrrbpy.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/giopoyaqj.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gayocwkmr.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkasnokwd.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gxyvizdmw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gapydnwqg.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ggorsrfxw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gihymmtdl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gnsxascil.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gpollnkbk.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gohunldas.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gfvvkcgul.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gfsnsylds.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/ginaemwmb.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gwrlfiepj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gtsusvkck.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gwhklagnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gufpkwvro.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gepahulqs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gattlxvft.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/ggldxwqoa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gwitweghm.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gptlxuudh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gzffdzmhr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gzyndzayu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/guzamnrht.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gfbduucop.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gfldfglwa.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gtxrztiop.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/grmnnyxdk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/glzqtnqwi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gsuskugao.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/geemqnyqh.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/ggeqpwtcm.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gkgwirekz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gfxnyttmy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gnayycgic.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/glakomave.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gcarswsuu.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gbowgldxr.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gwghvrsfm.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gaxvdnglp.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gpbqpmwov.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmbecvb.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ggbkvtord.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gbbehzboa.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gofkjnink.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gidtjklts.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/guopjrmtd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gzixqjaxc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gqaxjrnec.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gfgyentlu.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/grqomwdwd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkiedebwv.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/geyqdndcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gnlkdplta.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gffpzjzvx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gnvxriljg.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/geylfzaev.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gxgohhxme.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/glqzmtzzo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/grzcvdotl.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gfmviiote.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gzzdvwwuh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/ghetkmrzm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gswvicjwn.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gbynqpnth.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gwilzbvjf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gvrciczgv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gxrcgzyzf.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gwdybyhny.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gryrjdhct.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/ghudzshlr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gsmhnrvwi.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/ghdwovidq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gwjlkwfco.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gkpupwgjb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gfcbxgusr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gzhopwaud.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gletrgpdz.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gkabvvrom.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/glekvwiim.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/ghynllrde.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gofgvhrki.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/ggnjwippo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gshajpqaq.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gqlagdvsh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gmudhssmn.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gpozjnwqh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gryysnwwd.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gywvzofci.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/geobwyoui.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gbojjhazm.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gbqguivfa.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gqemtbyps.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcjgxgujf.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gfprrxbqv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gvlbypfnd.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/giofqruzg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gbfymhmau.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gyiyysjib.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gprdcpeto.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gzfefjojr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqzuwyetu.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gidmeuiyw.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gqtnivutz.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gyjibyeaa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gesilpbxg.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gakymgiwx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gwtxiqrsw.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gpgcdyyki.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gfqxhcxat.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gehbxgqkb.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/glcttnrst.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gfyaykkqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/grjbgkvmp.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/guztqpmgu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gohoisaqv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gcifhymfi.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gpyhvacmo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnyypcjdl.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gwhpikjsm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkvwrvpal.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gafmaspqg.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gtekucekb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gumryndis.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gajixijud.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gsaaunwrn.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gvkaaihyz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gbnduhkjh.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/goscdeyfz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gwisoryhm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gbgexrugc.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gxycrtcny.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gsuyrxzgv.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gwliiptxb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gkrxgkevw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/ghpskrpmr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/glkcmbpdm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gbrsysgst.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gsnahzctv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gtbwltivl.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gsfiztksd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ghptymjmn.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzrknwsig.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gxonnbcln.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gjkpgvkmy.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gufajlvbj.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gxtjqflys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gaomucreh.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gmrygllqe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gkvjxepwe.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ghoimyhfb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/guhhlvguc.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gckldpppr.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/guxyjmpjv.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gtearwgrr.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gunyzxkoe.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gfrgiaatt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gncltqodm.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gttpaucii.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/geslxcedz.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gbtejvpqr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gaqmshhyg.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gwlxfpaet.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gukloueuw.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gtamfaysu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gnxlwttsc.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/ggyjhjknd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gzcjorlyu.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/grrvjnplo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gqemwcdoi.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghtsrtjnn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gokxxlacx.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gggqbxmim.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/ghtmbglpv.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gigasfsbp.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gctxfvoyg.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gwslhoxie.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpzjixufq.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gpqilxsnm.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gncfccoib.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gccxaymny.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gwstleuuz.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gtoxpeedp.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gmgstejgv.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gjbgrnwsi.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gidgloaso.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/goqramwyu.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gadiqjzjg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gyikyqnoc.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gqhkiuima.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gofhgeyby.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gkeiyyjul.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gxvwvgeme.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/geiqqgedf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gynmhpxkf.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gazvhcpup.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvajlyhjv.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gdvfnamge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gemzfavcr.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gloqmscmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gcfulxiep.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gkpcwhvhy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gxcipyjdf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gymrbiuzq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gtkcpmnnm.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gdldotgpi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gefcyaygg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/geaoqeitv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/ggmqxtgmi.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gqwvtowaj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gtidjlvnf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/ggsnnwsah.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gmjnollvv.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gjlxrcwlz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/ghwmbegwk.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gwybmojwe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gryenznay.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gpwrhrtuh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gbxjrosnf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gopbrkrss.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gzljyiobt.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glbdwosso.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gkifrmogn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gyugqldsu.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/ggrruihuv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/glhwcpaly.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gkqkseiip.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/golgctugn.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gehzwmwuq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/ggczrzpfd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gvrbpipgq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gnkgjuxpd.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gfkqzsyzh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gkamzxely.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gevivemzg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gmevppnep.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gpnikrhgr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gwvrqpctz.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gkgudcodc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/glgfvpfje.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gokwsexep.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gnfheekso.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/grxvfwxln.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/glniuemhb.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gctrutzra.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/grztfwpfy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gqvfhhsma.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gumzdvavx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gatafepim.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gbzwyukik.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqvnzaoy.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/giupnnjbh.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzmazerlm.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gritmepiu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gcpxipthb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/glnvcdneo.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gaspfnscc.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gauqgkhvw.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gksyhhtzf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/goxfgylto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gsufpnkie.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gxenguxsl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gymnhcqcz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/guaidzrvn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/glswwlvuu.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjxfggrho.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gfnzehely.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gpjjqcymj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gagibtfrq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gcorrstab.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gfsdjnfln.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/ghegdxvcc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gbmgekqzm.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gtoactvth.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ghzksciaq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/ghfjwgtwg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gpkzhapxd.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gnhbjrkau.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gogpbohem.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gyfhsuuui.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gswshvias.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gilsgynmx.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/grzapwdgj.sHtML


<!-- 参考信息 -->