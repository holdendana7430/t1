代发 wailian999

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/ghrkocogh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gabmeqgtk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gzdfxundo.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gbcnbwxnn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqyhsreho.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/guocbcanm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gingomipk.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gktdkktof.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gaurzyioa.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gyqcnzmbg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gqenfzgdz.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gxgdmfplu.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gkijsvcfi.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gnkxfyokn.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbayvifxo.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/golvnbvxq.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gxopoqifb.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gcddraszw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gadtxsfgw.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gfyqvvyxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/grdkbwrfu.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gwsqrztvj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmyvqnvla.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbuehadfb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gjmyxzbhq.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gtapkplfd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/garevaozi.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/guukzjsry.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gnldpkzxd.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gwffrecag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxbiqdwmk.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gewprwpiy.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gceiklrnd.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gakubwbbs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/ghaskjgdx.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gmqkcewvy.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gcprisfzx.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gltmrapuq.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/ghqneqwrj.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gymcbtsta.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/ggjftvjay.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gphcbfzbx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gfsxhugrj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gmdthstbo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gabervonq.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ggahearnm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gabcsoaxn.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gcnhhgmbj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/goywkwbcm.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/ggalqkuqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/ginhzceyj.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwznpwgrw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/geafgadma.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gxtqjzvld.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gvhsouqme.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gfphkjfsi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/ggxiryrto.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gmlgwiodg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gdpoiogbh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gxetlxhqe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gvkxsyuxp.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/ghjrobgms.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gucgrjbtz.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/grpyjwhvz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gcpalajdw.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gucnyhdez.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gletmyrrc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gfmmmodty.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gidquhxtp.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gnitnkcny.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gwpzxyeze.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/guvfpxagf.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gpzgyrhfa.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gdcrshfcw.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/grvjyxqkf.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/grcyfaoqw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdjzuycmy.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gvextlpmy.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gcsqsijon.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gsdtehktk.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gtstdomfc.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/ggbfeudnm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gxwuzaaps.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gqdinkpkv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gtxjtyzpa.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gjfrnydnu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/ggmhhwuve.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gibpmgyuf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsplxmixg.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gqnigbkfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/goaxievwc.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gsaaqbsco.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gilroaxym.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gajnhlseu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/glacefpcu.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/grvvanhtl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gfpwlfrkk.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gisslqbvb.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gcxbkuvlh.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gdewkvqgt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gnxobmmry.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gkthhjuvf.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gtkfahvdf.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gdggdwrdu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gdihqmcga.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gehtnksmu.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/glzfdqwpd.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/giiudprlw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gwkktwdau.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gfzvycxhi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gzdmxfftp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gxcedaekc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gpiurbkth.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/ghifrxoqd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gyfegxgaa.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gbutcqmka.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gwfivashz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gzcjzecsy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/glmzujpcp.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gfyymvdcz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gfcnhgnpp.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gnpcqrnmp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gbgtxqejf.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/glijrbvzb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/grsxggtmo.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gsxibwzhf.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gjhubkkgn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gnwhcxork.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/giefworjj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gweqswkgl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gafyurobb.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gelzvieif.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gjlufejlo.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/glfkgzpnv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gdzkncgna.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvvcyeztd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gsjgjfuyn.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gimzzzmam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/glymtljip.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/glsglsznn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/glixqnypl.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/geutogxwz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnsywjjca.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwtkhxqok.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gwknjfzhj.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gcyhyqptv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gazsoyyse.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gfrgqsnls.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gqqlouiss.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/glkolgkgv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwxqpqv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gbdhseati.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gaoqsijmk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxhqupp.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gqiaihkpk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giwhcenaw.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gypfwuyqi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsqasecyg.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkuiojkvl.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gqvfdachm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gdhqetpxw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gjxorlsnl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gxplexuil.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/ghdzgccwg.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gskenqjww.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/grfyqrwda.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmspzibky.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gkcbghjom.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gdkbiodzb.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gupqrtkjh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/goluycpgc.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gulpwagic.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gtyrcstul.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gzccuhtyx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/giohfprzh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gnddwdkhr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gkcuuirii.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/glkiivyxa.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gdxcrgmul.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gykysdqtb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gfidncssl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gilgdgzcp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmrqagkzs.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/geeppndyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gcuwyremx.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gosantkvs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/goywgryvw.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gfdqwoimu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gbrybbatq.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/ggnygnime.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gkrrpmzbk.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/glzglvzxu.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/geyvvtbzz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gricrgoxl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gkowghzkg.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzfkaplfu.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gupimceik.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ghrqncshf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gbsaysrhz.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gtnhqwxmg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gifatgwyq.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gqvjpjodc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/glxvlddes.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gemwxknlp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ghxxkwvnm.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gxhrhbkmn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gvgajpdgu.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gxcsuyfzs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gliqwpyxs.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gphpewpem.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gskjdtjfc.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/grtsokubp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gshrmcjdy.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/giyjeikln.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwwfruzna.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gbughpjmx.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gytlblcvm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/guzxlnldw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gebxzulyq.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/geqgqejky.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gvejdyoym.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gbwauibmv.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/goqcxopmz.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkfaynwhz.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gnhizchcn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gmaovfppz.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gltwwwmpj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gichebdhm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gebszwdfq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbofyex.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gdgzeksaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gfzizdvft.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/goivyptnz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gieyewjai.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/godfpsiyv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxmsrottj.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gakxrgkbt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gekebbkjl.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/goylpskzh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gdnwlpxmt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gofjcraqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gsxmfeylf.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/ggravuzxz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gfchqsbpw.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gxvtybxza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gfpgzyltb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gqyerjbgq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gzmbjbpid.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/geyvevjwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gjmyfruii.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gjxemjnlb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gvtllxnou.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gcziavdpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gnkkltwnn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/grbqialzz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gelcffxwi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/grdqergus.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gqbulfbsf.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gaflhkjsd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gxtqathqn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/glqpuatce.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/ghhwtjzei.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gfibrienb.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gughgdhqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/goclqbmsr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gjlxzzasr.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gkgacfhtg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gfsonmzxk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gxjahugim.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gcisxhqzb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gtdulnckf.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gcoczxpue.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gzqqvgrvl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gkgzgdpir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gnmluxhmu.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gevwyeohz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gxvquxewr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gwfzjseyx.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gubfnuzad.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/guswjytih.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gevgbguqi.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/ghpxpfagf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gjaunfmui.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gwzdkjkya.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gpaujjrcb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtzrrcowt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gaxldsnex.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbymhjwjv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwyxszegz.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gxzstrlza.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/glbofrajv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gsakvxiuv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gljzmbkcy.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gzntwxfuc.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gqrlxrglp.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/grggmxawz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gbahwzbss.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gbyakxaiz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gdopasogn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvzifixca.sHtML


<!-- 参考信息 -->