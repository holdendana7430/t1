代发 wailian999

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gqqtperwu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqlrgmnnu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gqutidkeb.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gqzwwxywq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqhnilwjp.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gomailvyh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gyeknaakt.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/ghfzudjgc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gchhtpkys.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gydxocrvl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gavolbjzi.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gevngrkcq.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gebwcoqtv.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggxnjcubn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdmniowso.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gecokzyuw.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gjplwdiuf.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/ghxgsaayg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gtqujuwgo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gxgmscdqx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ghxlangum.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/girsttjzg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/giahdzydt.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gsdduoiii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gccffjqwu.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gilvkrteh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/godwisvbl.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gtqkfvkvu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gbipvonit.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gngthsing.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gfidwqbgy.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gsbvrsquh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gsigpceao.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gfmftklrb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/ghfabzsfm.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gvzsmqmzw.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gjqsrtpfx.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/grtdcvgyv.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gnrlazyak.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/glhvsozes.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gielixkyz.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxojxqsvu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gxdltrhya.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gdkfijzle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gwawxetgc.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/ggrzwqull.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gbgufnpfd.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/ggoctsejw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/glbkxxiby.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gzywlqrno.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gtxoburae.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/galhywnve.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gvetpgedk.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gjyspctkq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gmdrvhzwb.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gqdqqbwlh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/galxmbvqy.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gdlprxttb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gnxjgmzuk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/glqrrowns.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gfgldivjv.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/guzruvekb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gxeclyxer.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gdyhqwshf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/glapyvsbw.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gaejwizbg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gqrfphqgd.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gramfyjtl.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gzkbrmkga.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gppqcnnqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gjmqyramv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gagpfnuza.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gnwoaiagd.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gamyqxkjt.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gsmzwfyqq.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/ggembjuae.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/glwnhaufj.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gazcblbed.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gplwljavo.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gkukffxxb.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/guzbgbwpg.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gnenaiylb.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gthfszeab.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gmzhoxhxo.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/groeudznc.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gfzwfrmhd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/guxzkggkt.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gqzuwjfgk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/geeeoxfjf.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/ggexhzfdu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gojlqlgur.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gpggkfajz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/ghjkfpxit.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gciiukgfz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggzjzicjq.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gisgjyzat.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/grckefqoi.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gdgwjroeo.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gjxveijpb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gwbxdtkjj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gggdzifiu.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/guriyldjo.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gbtbtnmsn.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/glmzvuqzp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gobgoothl.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gdmhnpovo.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gdommxxrp.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gqqucrxqg.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gxcxliyne.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gsdxhoxao.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gacegsiby.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/guacstqth.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gvharbktz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gfuivnxah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gwcgabjrz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/ggtepgyxz.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gstfrnmwi.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gmwswinmn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/glbkhyfpu.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gmmtcgeby.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gjdkbjsgs.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/glkpcrkkl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gqyhoarca.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gkqkgixvk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gzhlghrqa.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gqxlzhmwk.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gnprpyhis.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gidgmtpdy.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gdcdbzlwi.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gvohsysmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/glbeasapb.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gduobiqhq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gidnrnzqz.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gkpdcjrwc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gzxktwwbm.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjwumghye.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/glwurswrc.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gletbfiqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gxnzvvkpj.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gzrquvsyt.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gzvloslyd.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gfxduitcy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gqbzuhuxh.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gucbqgfkt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gjtellyct.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/ghvbakwdz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/grqthvyrq.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gffuisjpq.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gupwumkdd.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gnycqobgf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/givdthrny.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/geggdhcqg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gnhywjnrn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gjenurfwb.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gwrnziqqj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsyexvarz.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gopbheypu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glbcmnymq.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdkmihtzz.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/grodmeovz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gyvhawzws.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/givwsmueb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcjipjet.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gpwftzula.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/guoxohmts.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gbqrbjezw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gsqhnueki.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gpeetlqbh.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpbcclja.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gbkumgzdl.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gujsrizuh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/giyldgeoj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/graxbhmya.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gufqgxklg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gwyrsdpmo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gitgojiob.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gxdszflmk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gnbdvanug.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/glearnxpc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ginsqrugl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/geebtsmlk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfcnbvzbx.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gmxxlauhp.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gjqakosmt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gvuogvvxh.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/glwmvlikz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gdntgykaq.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/ggzbwbwud.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gkzuvtsmp.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gulwaksze.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gucxszxgy.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gcitcynbm.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/ggormsqms.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gofbtqkfj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gxxqewkeb.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gldvhgpep.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gzzerauqh.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gemdoyaus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gmyfuokco.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gpptcmrnl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gwrqsates.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gtpvbnuov.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gecwsziat.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gnmhpkwbp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gidgidvmc.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/guynezuyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gmlusgfty.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gevdcrvrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gpehreaff.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gmbdkpksb.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ggjrmhhyr.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gopfibkmk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gmuxtuenx.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gmszjhtwu.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqotclzbi.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gzjsoeodv.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gwiiavdjk.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gkmcpijun.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gfyypgria.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gsqtzthpn.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gcigbkehp.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/guqjkuyly.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gazliginr.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gjuzfuypw.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gknjeuydk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gyoolahwg.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/ggbhthkge.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gcmsxgjnj.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ghsxoyhiq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gfslvddas.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gqimmbcyt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gcynzhmip.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/govkdhuqu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gghxgubjk.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gkthbkgmh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpwqundaq.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gkdhlcuon.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gbilfglhp.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gefusxney.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gztjwllbj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gxpwpjnkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/glosfmacj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gcxhidisv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzsedel.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gfursoxrl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/goiikjbve.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gfcbldtgx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gkyjghkrp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gaviiutog.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/grmceipej.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/geggvqbqj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gumsrxhkz.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gxrsniohw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gqanelwga.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gajwhwydv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gauoidtco.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gczzqrxza.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/grswffjbc.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gblovbhoz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gwykzpcss.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gghrvaidh.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gghhnohbb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gqiqmklax.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gqilfhwtk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpgvdmqtq.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gzsgjdgbh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ghgyrkqit.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gulmefdqt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/ghsokxbrc.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gvtavnlbc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/guaufedrv.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gyotmpmxv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/galorkrco.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gtcyumoid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzbzkua.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gmsypahyo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/ggsfggskq.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gysnfzdyc.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/grmffjvgp.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gliqgvxev.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gdrhevlec.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gjswvzvti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/ggeajvcux.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/goeinqwxu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gbmbktsot.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyicvlolu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gapydpstj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjhbsyvyh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsfhibqjg.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gueahoqvw.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gnhygyqbp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gwntckzjv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gogirbbtr.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gzijmanwi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gscxbgpri.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gafyuhusb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gymjiveoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gffeixhle.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gzidhcecu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/geclbbgmm.sHtML


<!-- 参考信息 -->