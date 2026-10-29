代发 wailian999

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gvzcjbhtp.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gmcjeixua.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gtnsaorpz.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/grmempzzw.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbytfespn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/goxxwvbpg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gfadyaanm.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gorcrpoyw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gazcwnvsl.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gipapxuiw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gpxfmkdiq.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gulztttlg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqubxjong.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gcxaupkmk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/glvogausn.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gwsyhswcj.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gybpzpzzl.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gzkbiyoas.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gscelhmeh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gewudehsm.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gqwgjokel.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gtequofis.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjuxrwhrd.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gebpuzujk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gybxwwrpw.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gjlyyvwwm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdgcdgyjb.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfvzvhfai.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gcbvjitdf.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/grdbxreeo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gokcjylfk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gaybjxdpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gddaswozb.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gzmcewkdx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfjctxpxe.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gotrndgms.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gtbqqnque.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gdqtrabee.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gpcwrncuu.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqqpwlx.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/grfyzhejv.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gjjkvdwsv.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gqlfkjoqd.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/goigraima.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gioxtiqwl.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gztmqbsrq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gruwnqdcb.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gpoyfhddp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gcoxxsohh.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/golmtbztl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/grvtwmyvq.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gkbgxkbrp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gktpeyfsi.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gqdddylcr.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gomhuqrch.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gddvexlut.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gdgcccvhf.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gizonckif.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gogpuvmlt.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gajjpjist.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gucqegubx.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/ghuhhiopj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gpmtvvjly.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/graewqkbi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gxpbnmddp.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/griivpxbl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gdzksvptc.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gpqfzaosw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gajjxwfli.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gpscogtrc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gkcapzwco.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gfaanrmkb.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gtokouvcw.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gyvtsbiba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gqpxacrhw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/ghwcmhuea.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gntkvntzz.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gbvqutvsh.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gnpqyvosx.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gmwayhlji.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/glgcvqqsg.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gfeuehwue.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/ghmcygzxd.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/guogmnsjj.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gzjaxcfcl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gqqlkuzbb.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gnnkncamo.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gnlfkabll.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gowvgfxca.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gvcfkfthb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/girksjdxs.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/glxoglnyi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gfqjhzndg.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/giuybfsbb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gbuvedlub.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gfhxgvhdm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/ghegxqpyt.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gdxcsvotp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzbjkqxub.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gbubtvuaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gntexgzby.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/grjczckwk.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gohbfsztg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gzrwguvqk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gqykhlvdn.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/goqppbuoj.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjgwuffsf.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gcelpisxf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gbhnywgbv.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gsmgubmcx.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gebjzmkvn.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gdshplouj.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gypenleqy.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/genjjjyvy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gaxxupyuf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/glzzokxkz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gbqoczfab.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/ggfefxtrh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gydpdosvq.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gmkmjlhln.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gvjaugotf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/garmvmfgl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/grebhknna.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gxxtmegrt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gdclfhpao.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gpgsgwpnt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gaijrejip.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/giqybmace.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gapcjcyyp.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gjguqhfno.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/glybnsqkf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/guovlrqmb.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmqirln.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gmvtzmxpv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggzumpevb.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/grfnjweqd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gzoouurol.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gzlrbidsm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gyegnqsun.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gozwnegky.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gygdaxclo.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gqljeyyzy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkeqwragt.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gipeyndmx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gcsevzfyy.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gjntaavnj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnpgxclxi.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gkkiblzpk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gtisohqyd.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gjuzwyrya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ggycaxjzz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/ggzlycsqo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/geotqruqg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gcufnuubj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gjksyvbbi.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gqvahjiny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gzffqdigb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqrealu.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gqcxnizgb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzdzymcqx.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gstqbqaku.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gucthwuvt.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gbxqwfshm.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gycfetpxh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/grltdrwia.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gjnovwaxu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gobzswtxq.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gbkdxyqlj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gwacyzcqi.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gsxetnjuu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gzuktexux.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gcejxxpyw.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gepzrgnbb.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gccuyengx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/grnhztsjy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/glwgmqzyq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gxspagjbx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gqvpilrpt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gdvsxlfet.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gajzovgdz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gbblyxojv.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/glmxdgzgk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gdcijxocf.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gpovttomg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gsxncdovo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gahghirks.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gqcxscemk.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/guvdycmdr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gfcmzgatc.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/grwdekwai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gprfvurrg.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcpvjodcb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gvoqhmfyj.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gbkeijghu.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gfhlvdruz.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gezgxdzof.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gvzkejzqs.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gywmmfqpo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxmkblg.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gsibyalhz.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gnaeicwxt.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gfcchhdxg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gakjkctjy.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gvxaicsks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/glvkmeyap.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gykoikefb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/ghgckuxbs.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gmubhtblq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/ggigztrkj.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gxatdrbnn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/glgxxfzrh.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gkcdxdkth.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/grgkbptep.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gilveqevw.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gzozunpzy.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gjzobxdsx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gecwhrdsb.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gawknwbpp.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glcltlogq.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gccsapdpm.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/grbqsjnbx.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gdkgsrdmw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqcdsix.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gevueitkr.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gmaasurud.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gbbauiisd.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/guuznonpg.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/giwuymtlq.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gjwcxudlg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gvskovtji.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gibctiomo.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gvsuhjgju.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/giwrfkcuk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/grbiktgun.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/goyxuwrww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/geogemaut.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gtrutlffr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqupubwgr.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gpftiwbqh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdfoybcht.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/ghsyrzklc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/geolomtdh.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gtmhesvej.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqbqqwhyh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gmijulygw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gpgngybeb.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gllmbbwmr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/glncgxdxa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghemjoehu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gjexpldaj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gowknqeii.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ghgrrsarp.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gdwzjtvrb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gpogypzll.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gdkrgeroi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gyleqplpf.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gdjehgaih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gtlhivbnq.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gkxpjzlll.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gachpegke.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/ghrxqrrej.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/glrbukthm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gckwuxocb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gagyynbxd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gzdwvwnks.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gthcfsjge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gziylvszc.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gmxhsywkr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwozwswlz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gtpadzvgh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gvzkdjdae.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gunwohyhg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gylhjbpcu.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gxvnusjkn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gonsvtljv.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gcireqozy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gcflifvlb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gqubmmytd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gaahopzqd.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/geozwlrkk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gmgjrzlij.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gjnabsioc.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/giutoqzsc.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gwsarokjd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gftttdjmg.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/ggsiwjzfw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gnqlwkpuf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/glbwdeymi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/guwfwdpfq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfscvybut.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfwkhwtcd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcjiuiqde.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtpmifuic.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggtokyeli.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/glqcmddgb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glvzjgomc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gmsnfdmnf.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkbcpvkuc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gscqqvujy.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/goxgztvus.sHtML


<!-- 参考信息 -->