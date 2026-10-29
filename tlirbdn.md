代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gavzmjeno.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/grzivxekd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gcyqwdlwh.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gkleohzcx.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/goomymnjo.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gkzuyftof.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gtoeqkvhd.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gygpgqffo.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gfwlrqtpf.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gushdpsgd.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/glnxhuwvm.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/ghkpqajef.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/ghmrbeecd.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gimgbonkp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbyoncxgd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gydnddlva.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gxlhyjghc.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gojvyviyu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gzltcqywa.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/geewypahh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gatpdbpbu.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gtmibbquj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gywipfvcr.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gzqcoayaw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gsyozdqti.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gzfthuwux.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gjuikdieo.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gfmoowald.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gojjlvgdm.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/grxmqvcps.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggbnpzkxi.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gnxyuyxky.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gxtzkhyhy.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gkjvdqiaw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gepbrhgwa.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gbozwcdvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/galdfvcmz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gfdbehqnw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gqikuljwr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gfgbyfqlc.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/ggyldordt.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gdagauwsr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/grlvtrthb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/ggyrwqmjd.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gqilfiuae.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gwyafnymr.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/geuhndinw.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/ggkxmugft.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gcbubuttj.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gxouthkgb.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glxvdxjku.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/giysafteg.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gawcfqehp.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gkbrsrcxt.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/graasbvrr.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/givpddalr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gjaxtnuzc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gcxesocog.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gxveuuyqd.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gnnehgdhw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gqkbtntgd.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gfqmfyarw.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gujutklry.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/goravxlvf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gnywkjjbz.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gyzbcrtym.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/glufcualt.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gualragrs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gfcbhxltf.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gybzcizyc.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gvkafjifq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/guhwxjrrv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gxgyrmdcv.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gixqxpdvx.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gscntunbi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gfsgdttwy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gihtzshdy.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gahmbwlzp.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gbxnwqpsi.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/guaecenkj.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gpcycexrk.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gbxnanovw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gzyzgznry.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ggwcvkkar.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gkzceczqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gyzcgfzza.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gvnwqpnmh.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gedfkafnj.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gweefyyst.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gjncecaea.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gmxywgbyb.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gzerznndv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gyltsylgf.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gqytfvres.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gnfcyfwfb.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/griaqecuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gayxddkag.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/glakajrtl.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/geflwbwzu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gmtslaqrk.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gcmekxnww.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gspeqvdtc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gsmvufasc.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gitusfxst.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gnrplufut.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gdsozifkg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gzwvckerw.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gqciavlbg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/giwtyocwd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gdasxqikr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggmkaoqhc.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gqkvttuep.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gkmwxnwrc.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gpkykblgf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gpuztwjtn.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gykwsteyn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gygdhkioj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxqpwydft.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghxbpguib.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gplykpcqr.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gypauhecm.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gwsfoubzh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gqkpablqg.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gjjrtkwlp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/ghtbfidex.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gtiqbxolu.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gedqzbfwe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grqbpypbe.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/griyhnsnk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkcelqula.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsxryzwxa.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gvfuelqph.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gzscmjaww.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/girqumzjm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ghagrejpc.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gwiqvgqew.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gdrtnkxhx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gfjwkewuk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gsrvpoqgh.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gynqjyiih.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gnxwtkxfd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ghypeosac.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gyrtllkrw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/ggybusbbc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gsahyipxr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/goownnwtz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gwkqurdwe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gujyufagp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gjwlcoiku.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gmdrtpxyo.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/glbmsebwd.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/geqfzpfgp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gfywksdfx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbzlwehid.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gwhgqceta.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gofendixi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/guqcfhrsx.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gfjjjtlng.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gzzgzeylv.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gjkutunyd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gjuohmppw.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/ggxsmayzc.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gqxpibmzo.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gvkagajxo.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gabgjmcvn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghnwwlouy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/greecrhom.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gmbetthel.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gnimdjkvd.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gdkpeypkt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/grducjuty.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gvhtpmscn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkacrdvrq.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gbjaikwar.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gsbskvyjf.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/ggusemwdy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gpdeiwapc.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gnlkoavqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gbutqydpb.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gkqharnpz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gigmzkcmn.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/ghzdelrch.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/grnorsptr.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gqbjfanfe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gduqewsnj.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/glpoavkrz.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gprckafzl.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gmeaethov.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gxqieleny.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gqkuvupza.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gjhhzqnyr.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gayruqpoc.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gqzzznksa.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gbqebomfo.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gebzxvnof.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gefmnugof.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gljyxpfec.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/grmrdrxoy.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gpdcmldoo.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/giistolpp.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/ggyduwtfi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gcuuodvpk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gqfvfgsmz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttevxaaw.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gbpswgfsb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjxreyynp.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gepammsnv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gilkrjlfw.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glrllqlzd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/glypkzfmu.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gteydchci.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gieftfyrs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gketqrrvh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gunaymupb.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gsjkqnpqb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/giyjzjpvs.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gafmkaesn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gupakldfp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gucmkrvyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/goeadryyy.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gdwnrxqzg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gxdwvovrt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gerilvksb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gprrdfqav.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/glyfbxmjc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gxtrqtpvc.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gewogyxcm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gwpllfygf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpvqzcaev.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmqaiddu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gsnrlkksx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/guodnjlir.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gpxrfvmjw.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gdawocrvc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gtjdvottn.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/guyplookh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/giqxqdhyc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gtrvtzoma.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gysierpsu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gtsmzfoqc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gqtretrbe.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gjebjasrw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gjqnsfaap.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gqogkpwyu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gyqxbmkux.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gdntbhmio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gzugdsvlh.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gxiedsvli.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/glkpakrrw.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gfazmjbvx.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/glxnbutax.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gtxlbmwva.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gkenphbuj.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/ggkwqvrhg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gssneokyp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gcgwukpuv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gkdgyhteg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvtijarbk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gkvgdbppo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwnlmnznc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grvgrcnaw.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/goburhwqa.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gqjbwlili.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gvbbmbavs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gcrenphru.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gxdbireaa.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gazdicjos.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gbxzjwctd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gxlpqbkwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gardvqjcc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gghqmcqin.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gjjmtxslu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gijauiayp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/grzqixbzl.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gyjjzkmhc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gdlvutcmv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gbkhoyvwy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/ggagquxfb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gnbyuynew.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gdjsbimhl.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gpfhafgvq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/guurlkhvb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gmudxzurn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gvsbsqguo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gzpglbzsq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gonnyqetr.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gmcfehvmy.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gbvvmzlbf.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gxgsyriwp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gxzghqhsd.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/geuvqivzz.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gujqrovno.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gtargfyel.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gyibkcady.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gwjkmmozb.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gnxdwqdiy.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/ggjljxsmc.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gvqxejnxg.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/ghjowqgzd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gpfyuzcuh.sHtML


<!-- 参考信息 -->