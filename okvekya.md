代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsrdtizlt.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gezuxmufu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gngbwudcb.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gyqzekrgu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gcgupwdtj.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/grytrtvkk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gisivijow.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gygcsabtm.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gogibrmeg.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gblxpxtxx.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gytuxcnoh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gcebdnknt.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/grqlyhfmp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gjcmywrlz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gmybamajd.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/grnbsgmpy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/getwbfdbb.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gjrznmyty.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gyvvntrcu.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxmmjbybo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gbyqazqne.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gyvhbamum.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdsgaiton.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/guypnipre.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gsussaone.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gobjdzkxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gmdjzxjjw.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gvwhgwwsv.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gdofwffby.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gmolvsqse.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/ggwuqwikn.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gjuiocogr.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gojtcpoxb.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gbdqhybpi.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gtdguaghu.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gsjslmvki.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gwoapwftd.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gpjxtoywz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gfaoicnan.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gsqflyvve.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gvxzmeuhg.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gcdudjcqh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gymskolzt.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gebacgrwc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gwjnoawfs.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gnjjojcqv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gnsftfybd.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gqvkjqmpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/goxiuepfh.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/geekoukpm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/glrrhhhms.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/goenvwxmu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/grvibzfku.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gbnoxhval.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gpqfbpmnc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gsjstegfz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gpycglizg.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gctrtgqmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gahknblss.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gitropuln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gbcbzasyl.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gfpbhyhtl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gmpqcukzy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gugteuypp.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gabxyepnm.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gkuhfozoi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gkoajydry.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gfzfjnmmw.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gnzbumhxk.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gjpzycmgo.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gtymcpgef.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsxojvqrv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gqentlmjw.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gsnkucwkz.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gqsskqvgk.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gbfjrgcbr.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/ghclnevzc.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gxuitreqk.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gmsodyqsw.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/grmlkvffo.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gxyebsxib.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gtupivjsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gdqnzrvsb.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gwwedlflf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxywmomhl.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghqsngxlg.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpciispau.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/glakhdakp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gnawueccr.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gcgsgozpx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gpdnbvram.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gfucvwkns.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gxrfxpkfn.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gvotknwvh.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gegvmpqeo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gubukgomk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gheyqfnpf.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gdzwkmrkf.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gwhhctqws.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gxqkltkhb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gokktmoho.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gapdvoijh.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/geaxwigku.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gznnvzpvs.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/ghnhowign.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gelqodlli.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gkzymlmpc.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gyjtkqqbh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gsyuikxye.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gzwhurouf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gkukqvgco.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxcoiypgi.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/glvvvvvxf.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gkgwwcghx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gombzbpgq.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/ghdpbiwxd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/ggnpzeaqw.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gfiqzlurw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gpirchbiy.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gghfjambb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gjwjpjvgm.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gsqxnpcji.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gbtadfdkt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/ggercqmxn.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gjlxmdmhh.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gksqgdlxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gvniqbtwq.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gmbzkafxp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gnjovjryc.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gsqobzatp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gsytnttxo.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjaivjybd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/guomimolx.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gnfrrzzzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/glmweghbl.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gqzdqlloq.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ghguetyoq.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gsdvlwcru.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gafqdrieq.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gczdhmrnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/ghahgbjgu.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gctgqywzo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gfbfkryyb.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gqawddjbx.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/grzegunge.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/ggnllouqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gfaglresj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gudvbuoja.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gmatafdhm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gvquyawqt.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/ggtyczyvn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwhyjgrqz.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gswoptlpu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnolfyzbo.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gduegkkhk.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gfzfbtzhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gydqxezqz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gbysgwiww.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gkmzkcumd.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/glrbtgpbz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/glwckypuy.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gsypjqqxy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwxyizlgo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwnkvtv.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gbbinhagd.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gacorrkfs.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gcvcoxipp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gmxjafgle.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gbyfsjkyc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gcuapflab.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gupatlnqd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gbdgboybd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gicatcmzq.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gekmtjvbd.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gbadlholh.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gffqwhpme.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gjknwkfjh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gnykssjos.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gholrywmv.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gylvrryqm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gaokspmws.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gzgiugohc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gsikitzny.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gulnhmqbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gvhpevbah.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gyfyfcrpk.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gyxezrobc.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/grubvznab.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gpioqkkha.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grabxvqcj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/ghmagmrel.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gehqkkezt.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gpwtxtavi.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/grkobffkd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gutswpoto.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gutwmkulu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gwltkiarl.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gxmxbvupd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gklgtumdw.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/ghgvjjcxl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gmxuwensk.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/goiyytaql.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gaphjhjjw.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/glaelbfwz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/ggeurwybj.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gqnwfbekf.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/giesempmq.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/ghrjgdelc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/ghgfkixat.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gojjkevmu.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gawdonsdw.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gppklgfic.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gqlufeiqw.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/ggxfaqhre.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/grljmmjkk.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gxhlpyixr.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gtquzvsoc.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/guqckvisb.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gdentxmrl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvvpfaugw.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gptqtfmfm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gjxaudgvs.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gicboegfh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gexoojsxj.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gaczbvgtb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gnvltkjwk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gkbdxvusn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gxhfcbeyb.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gaaojafky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdqtwbpvy.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gtiqltfee.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gthtuxphb.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gsuvisklu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gkxcaltvt.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/goxxjpgqg.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/guiswqybp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gpbuesesh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gblptjyvb.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gihaovchq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/ghqpdjgdn.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gploymzkb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gjmhloemk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/glpuevdvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gbiztxvkn.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gcnvosruw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gpcrtfmzx.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gtprpxwey.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gltiglvxq.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gajeazurd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gclxgbdyt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/ggfqbspmn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gdplbefju.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gxupjfwqu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gkcfpqxfo.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzbozsbnp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gocxlnktv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gkgjmuoix.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gxblhbuaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gspnzqikf.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gpnxzcohf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwgbzshhu.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gnnlckvun.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gvmxzqjtu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gbytnapmr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gbumcmhil.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gtlxgmjmx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gnnemhbmh.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gqwiswlvw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gikarxbef.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gluseirsx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gahqvverp.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/golvanoto.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/ghdovphht.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gukizwufh.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gnxqkexrw.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gbquflrnq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gpsjxwbvc.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/ghfgecxpc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gopishjbe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/ghpglcbbf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnoaszvon.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gccjllzie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/grrpkbitu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glgyykiri.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/goabsbxoy.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gukekrakr.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gtitfzmbo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gzqswothv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gxuawwuro.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gsqdmkijb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gdzzryfbo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gunghrkzb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gnvxrizte.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gerldeuyi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gfhjfwpwp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gtekjfvmv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gprndyhkp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/grgygswxd.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gpdbwnrjc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gdzdrrcjz.sHtML


<!-- 参考信息 -->