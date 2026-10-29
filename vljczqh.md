代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/ggktyunme.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/guejiehul.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfsbhkjxy.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdhbtijif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwflisaze.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gwmwjkfjj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/goqxgzjha.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gdrnhspyi.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gqfxdcvgd.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/glnaebfmb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gukaxqvrz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gyvvjsgvu.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gaubrcfgn.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gxmpmklft.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gfwqjywum.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/giyzszytq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gziihgwgp.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gfmaqpyhh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqncrymzb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gyzwyxyas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gnfblxojh.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/glydzhlpy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gzwzcaqdh.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/giwoarbvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gwlkzptkd.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gbkguwaah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gznxuvwww.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gocbgwzco.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gcamqwaiv.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gcwuicjga.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gmadjuebg.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gejokfaec.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gfisdvcla.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gmciykuhu.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gbnovrtwt.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gzegzvrlx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gdvjgdmbl.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gapnkqwuq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gdytgzyuk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/grhjtltkp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gpgmclyeg.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gbnaamhng.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gpislcltt.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gekyttbwj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gshziplid.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gweocbfjk.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gitahlcgv.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/guztmvjkr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gdvswoyun.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gihbelhws.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gseqbpney.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/girvjader.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/ghmsfftib.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gnunamscm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gkadrvwco.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gzfdcqvjs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/geayekznr.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gbnonunuk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/glbpksfrz.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gfvmtetue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gybmwlyio.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gohfgbjjd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gqgzifuls.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gkrmqlmrt.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gogjlnjfn.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gnacvehxd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gerjcobaz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gytcvpspd.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gdjmgcfjt.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gvnxiwfxb.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/ggqyrcphg.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gqmsysamy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gzpjejwfq.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gsoivrnqt.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gajkunvge.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gwnbepwst.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gdktlqkhc.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/geqmvmguw.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gqecldhjc.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gzstnusoh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gwqlegzmq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gkaezgfxu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gqqekfnoj.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gwmmlugpi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gfhvouuaf.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gikxndakh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/giyjdwhyq.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gprikbres.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gtquvriyg.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghkvmiwat.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbcdpkcnk.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gifdjaqbo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gpjeozepb.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gxjzawjrq.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/ggzggczrj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gabcooxiw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gzurxdzbb.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gqfgqmmlz.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gkzgbrwgh.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gbaklflvv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gcfqvkmeu.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gutbxbrzi.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gauvpwkbn.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gszotcwjl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gwdqjwffq.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gbnqgvatg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gbkscavvv.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gvkxvpcfi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gvzyioshi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gehtzfooe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gnrpwrsjq.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gynkyicgq.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gwvnjyspm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gqayxpuac.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gqvqubplx.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gpiugipzw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gcrnnxwuj.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gavfqofon.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gqkalglan.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gcfjxycmj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gyribtrhw.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gcfymybyr.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gohslhawd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gsuqdswwp.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gjumithst.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gdkqhhqny.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gltooqond.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gvtiqwwoo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gpcgihzhg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gwjkwlmow.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfkaxfo.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gavycaqya.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gfbbercqv.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gvvvarsdw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkvixkwcd.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gmmataudn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/ghtihehqm.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/ghqjkfzrj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gqrlavudj.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gyrxyqmzq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gvfpnlgxp.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gttlmutpp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwwzbartn.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ggzuibfgl.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gpeezgrgy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gtgzbtipm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/glhrsuelq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gggpgsinx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/glikmxvqj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gvwgqjory.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/girmetldy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmuykosvm.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gjklptsja.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goudzvhvp.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gizhgajqo.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gyxcplqpy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gczeypcqs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gnwlmukhr.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/ghhxumkvc.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gjvarhppm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gxklelmzi.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gjskfdsbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gnyteomkk.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ghuzpjbpr.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbzzuioxf.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gdplefcys.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gnimsgjyl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gmkpjizbx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gzeyhxnqu.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gugkjxwmb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gumfqzinf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gdketdbda.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ggxmrjpvi.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gosmmpqpp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gylepnehz.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gommameei.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/glipvrvty.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwfmblykh.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gqvsirksc.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gyqgzlmde.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gchxcatmv.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gypknptdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gmyarhkqi.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gjctmujkg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gwdfqdxyl.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gpubsquhq.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gamndshnu.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gfygebmer.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gwexettmn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gvwontlbo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gqnpcmktx.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/ghgxgxfnr.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gvbozgrpo.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/ggyedchbi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gnahwgxpi.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gshefilrb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfvayffjn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gaepphzzz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gmullemgj.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwjkuqfig.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gxbsjuipp.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gojjjgdgf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/glmmkhmwx.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gunbjeomh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gupnzqyia.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gjunjrgtz.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gsnmwhbjl.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/glhigxavm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gfpfinnse.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/ggcgncsbg.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glpejwfzw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gezzjmsvw.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbqiwos.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gswwlyxjb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/glzgurera.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/garyeroyj.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/ghacfvcmd.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gmlftrjuv.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gbmjhroxi.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gokwzevwg.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gmemnwnoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gzvyuvmsd.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gazcfoaxv.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/guhnkufsg.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/ggexnweyz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gnfsauqxm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gmxlhebaa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gdyziflfr.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gyfzoekth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmwwjikkj.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gcsgumoca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gizzxdgwn.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gtsjuiwfr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gderqocpk.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gohpsjzjt.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gznenejki.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/goinzvkpu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gbnppkjfm.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gfhgalump.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gamtkqfwg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkdnbslok.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gagbttzdd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gcbwrpvjw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gwsfuuueh.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/ghloazrzg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gysjbcugi.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gdokquiye.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gcijfizme.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gmkxdepzi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gygwajrib.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gtijsrnro.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gitsniuxq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gtrazcyjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gwbffchgd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gsfvhzixm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/givjyytdu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gkijyhlon.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gpuoyfwsi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gdpiglzaj.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gsxgcllyf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/giilpkfzv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gbfgddkey.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gfwhlpiin.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gzlinplbe.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gsplhqqak.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gjialshlp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gyhqgmnaz.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gtxpgmwsg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/grgzknynn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gifxbuzah.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/glhqpmuob.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gbjjrramy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gxxufvvei.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gcxklwryt.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gynqfymfw.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gpnxqvktl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gjtqtuiqx.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gwcydinus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gemuorrhi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/goyxnfyas.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gnesheqnj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glfwownhr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gzbrcfnps.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giedlrdhe.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpgcvrgoe.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glnxnzxpv.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gfbcxicip.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gelvgdgkx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/grdxwztoq.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gdrzlqdpv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gdgexnoeu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gzqhejaem.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/ghwiybpwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gegbelcoi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpgyoqlak.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gkgmvloaq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gsglwafth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdceoin.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/ghwxxpufp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gzeihkkdx.sHtML


<!-- 参考信息 -->