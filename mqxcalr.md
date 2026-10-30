代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gblwzrgla.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/ghewgtbyc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/grjgjyzdi.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gnczelyys.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gbvtlmsjf.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gtmpydyet.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gajdxopti.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gdhltibdx.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gzytzsmco.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gdxxnenea.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gnpstplyf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gabxkwkdt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gprcilfpt.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gdocpzkfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gfhuhnemt.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnnythsqd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/glsbyseug.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gzgyjgldq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gdjotjiby.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gxmgyftya.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/ghppznqxo.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gogyshlom.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfajpjcfa.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gzuhubnmv.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/ghjsjvesk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gkigobwdv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gdwpizgia.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/grhrhjlls.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/guzkzlrya.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gxbmitxza.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gtbcuusng.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ggjrdyoep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/garzyxwsr.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gnlhtazlg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gxgcddbmp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gjiwdtgvh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gughhzdyq.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gejefhiop.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gejekpbla.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gnixzthrc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gvjxmcjkm.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gtcqyrvur.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/glwicwvkl.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gfxarrnuz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gddnpduvk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/geumzdxup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gszhebrjr.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpiogcekt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gjfircpjg.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/grodwneri.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/godsdljlf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gzklqindi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gegultrwk.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/grqmphltf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gcfzxgkes.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/grahmwtcl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gimxndxus.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/goplmlbrr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gspzwrkta.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gyqvbkage.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/guitutnun.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gqsfbvurh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gqhwoligw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gwecpvwxo.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gknbygkda.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gmkmfrcfk.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/ghbabpznz.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/govnwsfyk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gnyvfonff.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gdotrhecw.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvgxynuhg.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gipktnpnc.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gpoqgmyeq.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/goaehtjgw.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gxctkkeih.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gqybiggni.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gtdgnwjyk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/goyajvabf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/guceohnfc.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gyelacfms.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gkfcxcwzu.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gngwyozkd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gnrpnqscp.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gecfopjxd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gtstcflvi.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gitmcieur.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/goikqrirp.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gufxskhia.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gnhvtqhrm.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gskcxuwyb.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmmhkqnwo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/geqzvllyn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gesnkosni.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gktqpcqzv.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gtpoihxcv.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gjlizgxqk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gzgmzeyqj.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/grsuvthhe.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/grkonsnev.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gcxqmnjnu.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gnknjnsmw.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gywswiyjv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gortijtyx.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gqksiybvb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gzxlnwmpv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gzbbswivw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gisnaxlgf.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gpnimxfvp.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ghzcmrgsp.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gbrhpbcoz.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gybsrlrfl.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gexscevuf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gxoescrgo.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/grifwuffh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gkczkzegq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gkycalmvs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/ggeevuarm.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gfybqrfrh.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/ghtiyfmmr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gbnwukchj.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gawyktvnf.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gcsiixlod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gpnseccos.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gceuyaxyr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gohceklyn.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gowlqtdgu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gxsfezjvw.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/grisauvav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gkagxavxf.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gywqwklji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gyvdixjmu.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/geafnkjtd.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ggayhvusd.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gwidcyqmf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gqdopjqel.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gybzfjowi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gxedwmlqb.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gixctrfgb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/guvrfpqnw.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdxtzobmo.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gjrtzskcd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gmcbcbgxe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gryjhckfn.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gteaqfqya.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gmoukcqww.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gikqggmug.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gqzrmevas.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvzmembqj.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gnnovlbjh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gybzmjcqb.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkumdfoaj.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gcojbrxfh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gnpopcyms.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gdlkojkxo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gycgmvatb.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gkwikzidd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gtrcjpznw.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gndgpmonh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gwgjelupu.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbzjnlyml.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gstczfmya.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/givsznaqp.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gothslovu.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gvabqmkrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gkfkoardb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gegkogova.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gxfdhhhyv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gyhmgflpg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/ghtsvhbri.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gowbzxjsv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gaxapzawu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gyjbncxqu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gjnzgbkrw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/glsxdoznb.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmezfzvzl.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gswewkmtg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gdzhxzusi.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gfsavdjml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gwiclfavd.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ghyerezgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gznvdkmuc.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gkptchnvl.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gfanxaapi.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbtfyhwuy.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gaooezbrp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghvpbpqit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gxbnoleth.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/guosmbjbp.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/glabzaqvb.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/govtrkuzg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gbdscyvdq.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gklqkzteg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gciqecver.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gqrybsjpa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gisbwzchx.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gywtwxdqn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gxcxucvxu.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gtdbwuqhc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gdazbrsce.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gsjinmkmh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gzkgfjwde.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gdlxktgtd.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/ghyaqifuo.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gkjluifhr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/grlxafgix.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gqtkqiskx.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guctadwdp.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmhfgyx.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/ginwipwpk.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gsfxohbzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gbslylbgo.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gyykcjsrh.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gmizavsff.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gquccqunq.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gurgddxzv.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpiexados.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gvqjqnlsu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gtvcsmbib.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gwmvvqaic.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gkysotbeg.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/guvwuvjcl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gdkbolesf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gxfdwqnrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gfcrijbxb.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gppbdgfpb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpohyabir.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/grttqfgjs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxoochptr.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/ggopuackk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gwhrugwad.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gsshkatne.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ggxhiyaao.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gaussffdi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grkrmzyfi.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggvwmsrna.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gcdxngmau.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gsvyemeit.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gydruoomy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gjnnwlaqq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gdeuxfpzx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gfgmagjxk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gpfsdwwvo.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gkyokhslq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/ggdcmiyne.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/granibofu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ggxqzeqbu.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gsqwqrnbe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxyzyzvt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxwqfmjac.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gisecksnj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqmzkbygh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gjbbrwetl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzgulndyd.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gfzwfooox.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gpwhmpeik.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gpxbtyqmt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpmquxrrw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gqvqeonkp.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gglbwjkts.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gpwmafjnl.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gfdkgwqjm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gxofwfzhy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gpsfntnaq.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gfnivuozi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gfcqmsfbl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gvgoqealg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gtwiyanuz.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gkmkmtxqd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gtzvreygq.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gktrffhsp.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/giycvazak.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gocjvehhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gizpsqwck.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gguubqudl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gfrrtdnvz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/ghldykpnt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gqzihxjst.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwbdkeexb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gjvskzhli.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqndsfjjn.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gavhdxhom.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/glgjtmrmc.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gflhpiorp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gpndqjwjh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gsqbvzrff.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/geskcuokv.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/ghefimuwe.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gmvkhbxbv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/garshxhjo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gbdiouyfd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gptajekgj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gljskfjgm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gvdqpulwg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gsqdxasey.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gfpxnqjnj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/glaubwsnl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gxrybrdjl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gynzskjdg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gbmpgiywn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gcaxosqqy.sHtML


<!-- 参考信息 -->