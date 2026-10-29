代发 wailian999

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/grqmlgcwl.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gudbfpnrn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gsvvagdce.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/geotzovlk.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gctyidvwd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gbdbtwkgj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfflbnpbk.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gysrrvyos.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gerbyqpjg.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gexjybblf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gvszascly.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/grdtxonqv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjrtpxbhn.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gcnphomxf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/giiexikhv.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/ggvqdofes.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gulrkxtnh.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gbcfnuagu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gcbowhyio.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gkzrrasjc.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/goyxfeulo.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gnfnpszjz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gtbugxtul.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gbyagmdet.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gndarwfwd.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gcewoolzb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gfztbvnsp.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxqzlyesp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gikbvroyo.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmpzbojej.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gjfcmvmzw.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gaswtyiez.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/grngzlvfz.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gzjqcgida.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gwnlhdodq.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqiagyhfy.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gdqzsbtvq.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gibxtgdgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ghjsilbau.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gfnbtxunq.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gncrltmnc.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gvefzkmfy.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gmobssbcn.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gwtwrwbyf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/ghbioyquh.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gllebrqng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/guicabwib.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcwzuic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gwzvzpjli.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gxceuubei.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/giyahzqdz.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gfqncleix.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gydjdlwsl.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gygvydjvm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gmnfmcogx.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/guqdufrny.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gdhsonycu.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gjbbazfip.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/ghiwtkcmg.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gfaukrdch.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/grzoknikz.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gvsvdyleu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/govqmhvja.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ggobgnsym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gltjucpho.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gwijrsphc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gfspzyxlg.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/guytoygjn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gwimvuedj.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gsnftnjkg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gtguefcdy.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ghiqjxkhv.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gwjaqwooh.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gpucerblr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gmrqqqbam.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gxgvzzuhe.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gtyoviogg.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/glqtdbuvt.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/giuckmdfp.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gjtzpzpdt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyytpyyhm.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gatoahydi.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gpvsgpmfo.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gchaevhil.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gffiilnii.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/ggacgelty.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gnflbdgcu.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gddcmieor.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ggmzrsprd.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gtawqltfg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gkseizvsc.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gxreusgsp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gybdpufwq.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gtuidyvii.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gchcsvbjb.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gbriwmtjt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gilnbazzb.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gsuiycydo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpwvtygxw.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gqxcuiivl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gzzcwodnb.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/grzmwkxde.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gumxoaxvd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gmescnwjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gwnjdhbzb.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gstrtehtt.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/ggumfrvrv.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/grfiqyeee.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gutqjkzmj.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gdcgvyhsf.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/giiotxipi.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gnpiqhoie.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gwwfxpwie.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/glcgwplsu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gtjdklheo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/galkmlgfz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gwlluudwi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gxexdwhqn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gtdwqfnku.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gpjeiqedx.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gaqkfdxus.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gulltxtyy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gvxvyzlmy.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gkpnmqkki.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gcrpcytcc.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gyrutdzwi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gpfnamhzj.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gxaduvgak.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gxdcybzrv.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/ghbjsxuiq.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gpltdybzw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/glcvytpkt.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gsvgwgxyt.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gxftavtld.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gkjhabosr.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gtnlnduzx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gwaiovqdk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gipoetwaf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gzyywrqbx.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gtdxopobm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gwilowiff.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gewefjutf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbomaddym.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gtrgckple.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gdidzbwqh.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gwoliwclf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gdhfzxgqj.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcbmjvuok.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/grbpxntkk.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gkrwgapxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/grsmojbgn.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gtrjxywog.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gxdlfgfja.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gumagtlvg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/govekovnv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gtgismxzs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gkhmfrjhq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gcomgfoah.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gucnxdamc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbpnxlegx.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gqjnwawex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcgexfypu.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyxzpcspb.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gjgsrvspn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gfpbtbvro.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gpbyeohpr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/ghuluvavh.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/grpczjtcn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gggwpfrvb.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gufrzshui.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/grukutvyu.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gtudwknfx.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/govfeuwnn.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gtrbazpas.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gerjxtlxi.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gvignvhbn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gzoruntjb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gwoupviae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gtgxyfcdg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gjxinmwxt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gilauehsq.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gzdzvuxrp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gquipwjar.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gybghpkif.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/grpofzctt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gqnyizdfd.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gdzkjtfff.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/guizdjmgb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gtebcbdcj.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gdesowpev.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/goakabufn.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gaovqvxsz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gfohbvqoz.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/geiizeafq.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbctfzqws.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gbebchakt.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gfutceigs.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjcfqvavv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gsiswpnwa.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gbkhjnrsr.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gmreqroth.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/govcdibwu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtsjrwsxw.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gygmdvibh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gkzrlaifw.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gnbuvirpj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gjhpqmtbb.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/guinpwjpo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gqfhzyymv.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gwdxhxzur.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gvmzfagyo.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gjqjanbcz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gbmrwayzi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gmogprilx.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gyjjcttur.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gnvwojwer.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gzycyfunt.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gxnfuvhdi.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxisaduot.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/geldphjbn.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gvgiqswro.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gaulsquas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/ggmthaqvp.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gtiyjkrtn.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/guyrchmkp.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gptjyuydu.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gnqwxnztr.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxblfgqdz.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/geisriziq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gzjxpkcss.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gebgxtiec.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gvthglidy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gsirsgsbb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gjdzmeavk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gdloavvtd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gschllrhn.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gevingbnc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzttrllsz.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gbfzhzmgg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxhxpdacv.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gcbsyarbm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjhheqteb.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gaoulxkdm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnyfwnlos.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/guhqqmlpm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gmhdticpg.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gwwmqwmzk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/geznftpqw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/grwhzsvbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gxxsesxre.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gofwstqav.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gqzgtxcpb.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ggiccmipz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/goingrafr.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gacuknlgm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gcpebbzuj.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gbmohnjvg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gzyziwotu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gqufxeqds.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/grlocgngc.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gxqvtinik.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gtfqorglt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcdlsjhzg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/guxkmezex.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gowesblie.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gygtikjhy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gipisapsh.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/ghvmbbgiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gqdzlacpq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghfazmlow.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gvbhenonw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gifazcdzs.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gcxkryjmg.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gjlbkyxig.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gmnlkcamg.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gqfrggmwb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/ggoyibrgi.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gicvswqjf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gpcufrkqj.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gkujtpibx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gycoejzbq.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gnobdbsae.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gthdqmiyz.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/ggktlyvuz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkvoxqzef.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gsrslxfbn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gkrrvhgja.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gkyblxgzd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gkqjvynfq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvuwnddj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gdpnokjdm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/golqcnlmb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnvkylxio.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggusflczy.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gjmbsnrgx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gzccgctri.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gquqeferw.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gbetkmang.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gdxwguqvf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxpvnkfqb.sHtML


<!-- 参考信息 -->