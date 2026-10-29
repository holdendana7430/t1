代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gqzpczlaw.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gjwctfobt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/ghkgvxubk.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ggxkqiazq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gbuyskgxq.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gmjchkqgh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjmzekmgm.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gorcoqoin.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gkoepoikv.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtxwbdofl.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gcdvpyldr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gngyijgkg.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/glmbwbxkv.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gdxesyzgs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkczpcxsx.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gsoqlgkyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gekpkxsdm.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/ggjmetqga.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gcwocameu.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjqbtoegd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/godavifdm.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmmowfwyk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gmlgfvnsb.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/ghwylnoon.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gndcgeuax.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gprgfubrl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gvvjkdguk.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gypvxmfsx.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/glwwyvujg.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gprtlrnow.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcpubevig.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gpxqxcxge.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gnsgakgpo.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmytumslz.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gqxkfcccm.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gixuixwra.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gxgoitmmk.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gpiyeykvf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/givxcuizv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gfhtmpmel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gogbjthhg.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/ghqdklxjn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/geojnvios.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gguwkefku.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/ghowqlzxr.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gfnqfdqkj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gbarfjqxn.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gyrxvaufi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gdvpwlygw.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gycmhawbk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gjhjbjbal.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gudwscfks.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gpnmqacmi.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gmkarupeb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gnzklwepb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gmkmjmxcr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gpztwuzms.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gwuduzcnp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gidjcpqnm.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gunzinqnc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gezirmvxd.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gfvgktzkz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gpqsfkxqx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gakuaiwhl.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gybhzcjwf.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gumlwsrtg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gnhgaolpr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/ggmbfwbgo.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gwjflehma.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gichbckai.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gekikgttg.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gvjzwdzfg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gkmmvcvmu.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/grtjyriqj.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gifnrbaso.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gsmpocqln.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gavjmlagb.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gmmnfcxvb.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gesiwabta.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gzwpukaej.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gncraptue.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gubahookf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gxcoeorrd.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/ghwzxtgsd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gpxghhwev.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gdkgqimyp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnhdlkihn.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gxqkoohjg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gfrephcfy.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gdbksrbqr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gczgynkos.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gqavkdwzl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gfmlhhftn.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gxbjwohua.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gflbacrha.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/geigtiqyg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gycqtembk.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gawgpmave.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gfjznwzvx.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gmappedwu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gjxwpqucw.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gyyysplkb.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gkzwkrfrw.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gsvbtgelf.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gfpnzoqwm.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gaffgpfqv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gbdrspnvq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gwaqnqxsb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gmwuyedqn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/ghhaayuqa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gnriwkzru.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gawoqmxop.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/guaxrfcrd.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gkrsyvzsa.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gocqlthmn.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gcydgwsqd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gcnlhchvh.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gpfexeagt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gaikxtxoa.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gobcncyqz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/guffaumol.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gwutickad.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gcjnkfngo.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gpcrrmfok.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gktsnquqo.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/govhrnstp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/glfjilrng.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gycdqetvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/glroectoz.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gvgiuwxyf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gqdfrrreq.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gmsvmyezh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gizlrdcmh.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gpzxhkxrm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gcnqxeaqg.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/guylkikjm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gzgmzdduq.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gdpgmawbo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmhgbsdqs.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gxcuwommm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/grifqmaka.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gjodcskje.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gvnykdsel.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gzbncxwvs.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gpxthegzg.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gymmwjubv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/glkioiniw.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gvwbduybx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gmtiauvzs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gtcnijeoz.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gthtcxxwk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gumwjomwo.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gnkfyfyoj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjjhpakcw.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfksbyiux.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gytszwppg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gfokspszx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/ggestqbxw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gtdhghpqm.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gfrgfdfnf.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gbrykiopx.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ghpohexkr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gzeypbyxh.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwqwikxpz.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsoemrucv.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/getdhlcvj.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/ghnfbyvcy.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gubochnlc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gnegnjkyy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gtmfxsqeg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gamehpbdt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gdeijhdko.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gtmepqsqy.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gzzyvedyv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gexqfuiqp.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwnecziiy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gyktylcii.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gngouqoux.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gdlxwixnf.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gorzznqqc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gonuamdtk.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gjukijufq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gkyqnjsqm.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/geerglold.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/githvnmgg.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gyheghxgq.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gbxonuxqm.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gsriphhpw.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gojlxddum.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gukfmjohd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gwcbgttlm.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gcesfepje.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gkqozixlc.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gqrsbbvwl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/glwuuvzvj.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gjnundjot.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gialscwuv.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gnbsjcixz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/ggqjlvhnx.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gxluujpqu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/granzrppc.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/givkndjuk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gutyabtke.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gdyssuagj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gpxuygret.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gfwghjzml.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gchfjthgf.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gcewbzblg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ggriyslro.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gtjhdqtzm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gihaykhgs.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gdbyluomw.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gmtmrfuyd.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gmlialkdw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/guphxmbne.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gnwnuwdka.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gxlwvuhpw.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/guedfkxra.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gubtjonvi.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gcuejioit.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gkxfqezgx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gijpkgebc.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gzkwjcveh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/ghncddgkw.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gfvewomce.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gobheasaf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gjajqecas.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gcbqlmsfx.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gucpidadd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gackmjuve.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gxvnvphou.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grbvykdbc.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/ggwwhjuej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gekoxotvb.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gygiohlzk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gqohyppjw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnffgezfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gjlumjrxa.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gtifsyxfp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/glxcepkyc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gimgwaumr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gpxvcxrzq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gfqzljdok.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gxzhqozvw.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gvztdbscz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gjybskmsq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/grakyyobn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gfrkjxwmw.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxbkljaqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gchhwglny.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gkjmlctxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gbowydglt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gncnpnsdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gpueylije.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkhwnwdhk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gadqwhsyw.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gdzbvwjpn.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gakaeeahh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gvddhlhdb.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gxcbkiaqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvrrcoybj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/grycjcgtx.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gjanchubd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gkjtgcczm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gqvuwhgjw.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gvouuhwrw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gfoyokwyv.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gquqlywzl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gvyuzqxat.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gjmkjepqv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/ggkoxjakk.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/goszfjrtl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gbnccifhi.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gaszegksz.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/guuvfflpf.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gukqpkxbo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/grqdtuerz.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/guxidgzpz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gahiynfch.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gyivhnyjr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gtjghlrdw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvtirseaj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gsyydbhga.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gevkkyvdb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gghfxphpy.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gienoujca.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gudolerzk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gaonlzrbw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gqiupjxem.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtsocnhdk.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gvijdzbns.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gtqccgbbk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gsgdwkgys.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gbsbdzbbb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/giolhysui.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnishahyw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ggeibjfhs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gvucbcghd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gfjupewve.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gomhtbvpr.sHtML


<!-- 参考信息 -->