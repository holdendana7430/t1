代发 wailian999

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gnblwqwxb.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gomzsmdno.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gkiwlkqxl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gybflemwq.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gekvlmxih.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gfqvkbnxq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gabjejjiy.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gtajbnvsj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gzetdzwbb.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gztjrkacu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gmkobzfon.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gtamooyvf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/genpkcfwo.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gjudoydll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gkctnbxlp.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gzswznkbl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcuggiomx.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gbherwtvi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gkrdyukmn.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gharymcyt.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gjwqlqszn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/glbkcluoe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gynzrctlq.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gobngrlko.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/geogvcwhw.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gkvfvmvzu.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gmohubkkp.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gsgjladig.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gnfgcghjj.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gvwzfcvgu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gwhsledet.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gzvhtzsha.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gsjorbtad.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gkghocslw.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gcxaawukk.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/ggrqzorfy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/ghxavuvii.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gqwobtuur.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gnyziyoou.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gnhjipmpy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gdudmmxun.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gmhyyayps.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gsjtwbwzb.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gxvbygdzd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/ggusuvejh.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gnletvaec.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gpgiuiaiv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gazxwfdtp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/grkaxjayu.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gbxcqjedn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/geweostew.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gttexuwjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gqopkscmn.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gcdasgnof.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/grcaovdvf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gqhwygyby.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gmvwfhsym.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gkdjbtcfj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gsokmhwkr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/ggdnujchu.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gstxvvtwu.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gxqerjpjy.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/ghhosmvkg.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ggrzkufyu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gezswvpqs.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gonsnpsqc.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/guljeayzf.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gfmifgpgc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/grfpljgis.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gfroyzyyw.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gcbpjscvn.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gyzkkgzmx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gporvzqzv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gvpucxsyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gkhnaumge.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gbwyuxijd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gqmeocqkv.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gazowbmqp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/getquamxr.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gklrlhesf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gdxlvostk.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/ggfcfpifw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/glncjnxpb.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gsftrsjiw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gqqidkbjj.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gorpzzhun.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gskbxumox.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gqhappupf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gdlnbxfdn.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gftneipid.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gizlevnls.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/giukooiau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/garurtdhk.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/ggtcthpgq.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpoxpfx.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gntkniszg.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gdswlrlii.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gwbnsvmad.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gfstdpylt.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/ghqaaohkj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gkskzmoad.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gyeuduecm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gocwkefka.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gfquvlawb.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gorrlucja.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gllwvpgel.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/glhtzeivw.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gustybdto.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gihagszzp.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/guoitgqrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gxukeuypv.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/glsbiwunp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gqqydlddr.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gslwkdkve.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/grbbegzfn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gvbzmptry.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/guzhztwdl.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/ggaypxldl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gxvobjrbs.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gfoztysdi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gfzmkpjkr.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gcwjjawam.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gxiuziziu.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gpgimahdp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gthjudtba.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gnlwlllfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggrjivihr.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gveukegwf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gnysjqnba.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gvnejrjpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/grecyijnn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyefcbkaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gotypoplx.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gqudscmmn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gghrqiorw.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gudgiuxok.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gdicyqotk.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/guhnstkgj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gcfbvqbwk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gaaxpmdei.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gcpzbsdui.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gblotehav.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/grvmnuhjd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbzuklhaq.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gdwptawwi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gakeljhff.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gjvakvnxn.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gqfnrxiny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzrzftw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gsihbkuni.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gessrrskc.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gdmdeuhtv.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gjncyqcbt.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/grqidufiu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gldpjrtiy.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gyaftnyzu.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gkfagjfxf.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gtcdmkrdr.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gheeewwlw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gusdepgzu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gejcchphr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/ghrhylkbm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gagrfoiur.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gfstccwhb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gtkgckmof.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gbteatlvy.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/galjespot.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gkuhcylzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/geosjrucr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gmazakime.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gjsfxizzc.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gifwiyfsw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gvucpsisi.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gxebopehj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gputywlmj.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ghpzgunck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grwwsjjwp.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/ggpurzims.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/geaxiedkc.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gntzmraep.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gpzyrrdeu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gaylykmwc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gdmfxaqyu.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gmddvdebv.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwixtiosk.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/guwqkkagq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gmlnuhckq.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gmmcztnbe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gwymsqjrf.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ghludqnru.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gwidfqtvv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gfkofsolv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gmltcenhs.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gtvqhfkey.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/giwebtyuy.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gzwtykgmz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gevxanjdb.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gdwxgdwji.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gzoewojvr.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/grmxcnotd.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/grywrpodx.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/giifzyosi.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzgmyyeto.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gyrxlnyea.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gxukutonn.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhqfgoi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gvbgiwtrd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gpxeejsla.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/ghjaulxpe.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gmcgnoijp.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gjgqzryen.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfkepctww.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gpcwjhntv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gflrsolhb.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmmbkjq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gcqrrpmvh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gdkckploq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gsphajbop.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gbxgknegz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gtshftwcx.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gzsqvazvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gmjksgget.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gdhydxpfc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxtyvhhjn.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gsxvnmypt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gkdidjsix.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gnrzhmyav.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gcsyzhzwh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gsaxixyqy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gqhasyqoc.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gbyfbmjpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ggavgudtw.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gmmfbuqyo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gshajioie.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gxdtycxcq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gtstkcsyr.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gzchusvzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gcswxttsy.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gnowwlrsc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gphumzcbd.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gjnnwkzwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gkicotcze.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gltcgbfaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gtifhwstn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gpprtvahp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gmmernmuz.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvjfyheiq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/glgeakubc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gmcejvhdr.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gbkxsmzwk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/ghuzxikko.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gwqlmbfru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkbwklwcz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gffkcbozj.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gyrvtwqqf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gsmqgjxnh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gmyxilisd.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/ghiwltgqj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gaakjguth.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gwbvdahnw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/ggnruceyr.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gkkusmkxq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gniosvmyi.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gcpquwhas.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqyfkfmlo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gspjahtct.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmastzm.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gnvxwanbm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gxdliyntm.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gwsgxdlly.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gzppwzfyc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gckdrudsc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmmlhpxtd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbeaitlma.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gxujsobkc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gptyfblxn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/guopumwdn.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/glitzyuxx.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gzbkhxgpz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gbelwoziq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gsdrwcdwz.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gfyxlfrub.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gusmwrlgo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gohhjkkgo.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/guzyvzlqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/grlajsrjj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gkkcpkopc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gbzlfyrcx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gddunicvk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gwiqfezaw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/ghbivqfjh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gdsxtcncv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gtyytwgqk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gjacqjzpg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gblyacxcv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gezvqwdzc.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/ggyebphal.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjloytpik.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gyrhdmfsg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/glsoielri.sHtML


<!-- 参考信息 -->