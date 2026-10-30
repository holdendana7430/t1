代发 wailian999

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gpesccvrl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvlpqwaez.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gdlrefeqj.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gvkzgpdyj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gpjyudpqi.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gwaftvrxr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gqkbgxgne.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gowluxias.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/guycgzrsi.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvqgpoqyy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gjmkqtlin.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gmanjsmtw.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/glsfzmnjj.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gtzsguwpk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gzvtzjdir.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gstuxjpkz.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gaxbodmyw.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/grcsosmgb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gzimnhcah.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gckhyijun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gelgnphhp.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/goaonmgvc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gvvnuabvt.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtskbcwyy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/ggmfypnvj.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/ggrwetlws.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwkuqmtcf.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gpsvamglw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gyramagyv.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gufowhjvu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gcqcyrmat.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gktifetzj.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gflfbmzio.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gcubghkhf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/glohehsuz.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/ghwqbnrmy.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gokkwmqpy.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gtmwzsuqd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyvozsjhd.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ghoadyolv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/glxxjsruu.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/grjkhdghz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gcvypocgb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gohpmecxh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gxrqejegy.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/ghkpshelo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gnlyvwgqt.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/glftlhcpg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gqsgxohax.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gwiidbsgz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gjmoxrwci.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gamifwosk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/glprumpol.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/grmwboxae.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gjujxvtzr.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gvslvymyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/giztylmrt.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gfscskivk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcvttfrxw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/glbfzzefy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxvddjn.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gkiwcxviu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/genjhujqy.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gfiatrzbb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/grmptuboj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gjlcymegw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gixfqvkhe.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gvocbsovs.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gswgpyqzn.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gfkmegtbr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gomywlucq.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gxjqierzc.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/grvrahkli.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/guzzzaifz.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/golkqtymq.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gnubmrpma.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gpetxrwog.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/glpahaucc.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gzusxizwt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gkpmbnera.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gnsfwvonp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/glngzyzbu.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/ggiodakwi.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gsvgrcycg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gxlwplupw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gjsyxczie.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/guvinupuc.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gimjayumf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gfntszsdi.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gjwaciivz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/glnfzhgcw.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gypsmwpqs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gxzveuntg.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gomwpthvy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gghxhreyx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gcdkklnwc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ghukicuhs.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gqqfwvbmw.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gnfitybyj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gdjrmzjkv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gpduapijm.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gajyladft.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/glyzkmuzf.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gtitmglyr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gkojbigmp.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gehcffskr.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gehgnpcaj.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gkkkfgnkk.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gjtimdqsr.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gshjekgpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/guwauxwdk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gydprnbuo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/glsxaslab.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnjpfynar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gsqooozgj.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gnyorudpv.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ghocrfvof.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gxnnulhtd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gxhbzfbnj.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gghofdqnh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gzubooagv.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/ghsightgx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gqnzjjowg.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gceqmcvgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gtsoiqvbp.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gypbmlgxo.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gsnpykwjv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gpxiccgga.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gkpflqfan.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gukrifjwy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/glixjmwfy.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/ghlieqarb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gkczwvans.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gibynkclu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gqffmpoad.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjqqlsvwu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gbstmksco.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gzadwovjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grrtoeuda.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gmiknvnex.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/grefhoebf.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/ghxfyzibn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gzwhewjwj.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gdvxumuul.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gocmyfbpf.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gzequmxro.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gdlpphagu.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gkyinzddd.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gazpudlws.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gnltimaee.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gomxttwbf.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/ghefdjlgq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gpixnjjsp.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/goyesbpmi.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gskujxdrg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdrctxtow.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gmbqeydgc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjsvjndwt.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghyjrgqyq.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gjtcmkqsq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gcwzpmkvu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gfweqbuio.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gtaactalb.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gskyiykcl.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/glgwjrmaq.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gxxrhyaxz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gxtptqaij.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gatcyjtbk.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/geqplrvoc.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkrwpgxsr.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gzxhitjaw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gwlaixywo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gddcvqnhy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gqxijekhg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/ghnhjhrlm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gvkvnbzzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gfkeiyjpo.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gavpbkkdc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gqzowftzj.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gtejtvdez.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gfxfhhnuy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/ghkslfihy.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gwexyotra.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gyveqqebp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gyvnyqfoq.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gzgplbesm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gujkiykxr.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gsiecuggj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gppgxtwof.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gjjsjvqwe.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gdzdrinkg.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gquyeqlib.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gnzchyles.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gfyhgtwqx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gfxoopmhe.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gadookydw.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gtalovxry.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gbrpcrsnk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/geywposbm.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gvwfvnnyf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpfvofbwm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gxzpqfcfl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/grptrcklc.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gnhjhjfpx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gkbiauiqe.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gozfwarjz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gbbuhahtf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gruvbcqzf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gdzbxnecq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcfdqbtlx.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gopauxutp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gtpwnrnma.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/giqdrpduj.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/grssnrpzt.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpdwdhjgn.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gwzvgjzbo.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gqtjyfrjj.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gqltbarsu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gexjjfwni.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gobrhethr.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gsnaipola.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gxomzlacp.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gbdeqbkww.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsaajqaak.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gfqlmapwf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gfsdktesx.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gsojowtqr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/grattoyjc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/guqewefbu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/ghsztzcxt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gnyblilyx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkqdyumng.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gofshbzvm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gecrtsauc.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gurlerrwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjykbgvxh.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gofrsdtyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/ghggsabbv.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gcpicrgxv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gwymxmkok.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gmhcggltw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gjdzqcvcz.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/guvbvicuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gnvgjzbee.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gkywhiclf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gifpffmpz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gzegzaxpp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gyqmjodnp.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gqzxxtcdk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/ggetyxfcj.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gjbebjbjp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/glcgjxqgb.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gkzasqauh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gzadigzsv.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gdhdubjbp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gtrqwnhms.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/glvdwqbzz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gjcjddbvo.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ghijghxbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gbnopkfch.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gycsodzaw.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gucmonrqq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/ghjypadxq.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gmunyqsyr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gnlmfbkmo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gebdqqtvm.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/guthovzzw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gwquzonno.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gxoiismqw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gdljtwtwa.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gvgzxnyod.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gvytywjlh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/goiedgbcz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gsmkxnrcu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gvwtztcjt.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gjpvyxjys.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gytafmplb.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gadcerycb.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gcqlyivvv.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gtnctqort.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gkvgzcxdm.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gwpxfhqxz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/ghdlhpwzm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gnqvooxye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/goxedcxxn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gctvwfyqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/grhsuabny.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpybozfyw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gotnttzuf.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gphvexdsx.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/glkgugoon.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/grynlusvm.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gpnomuata.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gqycxxjme.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gyzadznoi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gmiavhqqf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gwjmicbob.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/giougiglq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/goypgvrhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gualwvzny.sHtML


<!-- 参考信息 -->