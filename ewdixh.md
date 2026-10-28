代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtcggyjryd.html

[R08] 数值比较
来源：http://hz.yj202588.top/gtvzoypvoh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daxiang520.top/gthqtixikk.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtiwebpdpb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtekuxapdh.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtosqhcqbl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gthivjtqno.html

[R11] case 多分支
来源：http://hz.nanxinkj.top/gtxebsjdvk.html

case "$1" in
来源：http://hz.dianchejie.cn/gttsgyakir.html

start) echo "启动" ;;
来源：http://hz.bjfxy.top/gtdgmsylzw.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtyznkyuda.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gttslmcqln.html

esac
来源：http://hz.wangdashe.top/gtlpvnbqog.html

[R12] for 遍历文件
来源：http://hz.ywan-chungtsiang.top/gtmegfrdtc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtklljgawh.html

[R13] for 计数循环
来源：http://hz.jiagoushi.top/gtzkrzebdv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuxming.cn/gtpaoenjcq.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gthuznyfki.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtfxyurket.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtqecvfgdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gotoacloud.top/gtmhfrmxft.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtglejumcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xziqi.cn/gthlklsakf.html

[R17] 数组定义与取值
来源：http://hz.zycfv.cn/gttuutwduz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtnptznvtc.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtjykicexb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtbfattgby.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtlclrnvtr.html

echo "${#arr[@]}"
来源：http://hz.haohaochexian.top/gthwwfibgu.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtwgqtatll.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gaohongyu789.top/gtdakgouew.html

[R21] 字符串长度
来源：http://hz.guowangkeji.top/gtahgcfejr.html

echo "${#s}"
来源：http://hz.jinqigfzy.top/gtmvpwojpy.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtkudnsvco.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtstymdrjx.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtugapsrpz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhongyouzk.top/gtvrosenlq.html

[R24] 大小写转换
来源：http://hz.0kj1m.cn/gtxdszkxgu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtntyskkbd.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtnodnhtjj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtfzrleyfx.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtvcgdxyjh.html

now=$(date +%F); echo "$now"
来源：http://hz.chenjidiqi.icu/gtzcshqnyo.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtqshgjtgn.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtvhovdljt.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtwvevhoew.html

echo "scale=2; 10/3" | bc
来源：http://hz.tanke756.top/gtyotltrqq.html

[R29] 定义函数
来源：http://hz.shuidangran.top/gtuwkorbnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dashuyun.cn/gttglzxede.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtrfverdnq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtvzhtbfuv.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtkiwqpfyx.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtgnnrokzj.html

[R32] 参数个数校验
来源：http://hz.gzhubu.top/gtzitwskft.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gtfpgftuhu.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtvkanzunc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gthkhjwtey.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtnbkiginn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtqpqyvtqw.html

[R35] 后台执行并等待
来源：http://hz.meibo888.top/gthjxymddx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gtcgucsygg.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtwcmappvl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtjtvvjimd.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtkyizpzxq.html

files=$(ls -1)
来源：http://hz.mhx1999.top/gttnivdaea.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtydmvuzwv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gthkmorkwa.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtsmoirqta.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gttlceuaoy.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtizewvxit.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtvrthmtpp.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtxhebyqnc.html

cmd >/dev/null 2>&1
来源：http://hz.nanxuanxn.top/gttmcdqvjh.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtfafskugr.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtprjillxo.html

[R43] 按名字查找文件
来源：http://hz.wangdashe.top/gtardslntt.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtgffornrg.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gthxbnyobf.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtsjecocjq.html

[R45] 批量删除
来源：http://hz.ydjk.org.cn/gtrbmiznxk.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtrvpuekud.html

[R46] 递归替换文件内容
来源：http://hz.jqgfzy.top/gtnvhggjmo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangkeji.top/gtkhxyvjwk.html

[R47] sed 单行替换
来源：http://hz.tanke756.top/gtzglesukl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinghuilouyu.cn/gtvoefprru.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtogwyavtg.html

awk '{print $1, $3}' a.txt
来源：http://hz.gzhubu.top/gteshynfas.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtpkkvhdpm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtbycovyst.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gteetbklvb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gtahwuqwwm.html

[R51] 排序去重取前几
来源：http://hz.jqgfzy.top/gtvlhxmnal.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gthyfchhkr.html

[R52] 统计行数
来源：http://hz.dashuyun.cn/gtwyxfivxe.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtcljzhiyz.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxuanxn.top/gtqjkzkcje.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj202588.top/gtcvpletsw.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtwainilyp.html

diff a.txt b.txt
来源：http://hz.svipenyu.cn/gtrgzpuljd.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtrbldeoah.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtfgnryeuv.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtdwcbxxxi.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gtrxinfgnj.html

[R57] 远程执行命令
来源：http://hz.dianchejie.cn/gtltsscglw.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gthschuwdn.html

[R58] 下载文件
来源：http://hz.birdmap.top/gtyjoociwa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuanzx.com/gtmcwqodyt.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gtecjtpqhy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ehwqpu.com/gterxgqgoo.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtszvmpxnr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtvkrpnqfk.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtqipuvcif.html

df -h;  du -sh *
来源：http://hz.yvedp.cn/gtbdpzcioq.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gthwmygdtf.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgfzy.top/gtvzdppqwx.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gtcaqdzwuh.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtehoevlhe.html

[R64] 结束进程
来源：http://hz.vqdsnc.cn/gtrhxkxwnk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhoulong.xyz/gtfhbohqvi.html

[R65] 查看端口占用
来源：http://hz.zycfv.cn/gtuseqhmue.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.9152youxi.cn/gtomybjthn.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gtkukeimrg.html

crontab -e;  crontab -l
来源：http://hz.guowangkeji.top/gthbrzppss.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gtgecviajl.html

openssl rand -hex 16
来源：http://hz.chenjidiqi.icu/gtsblmxjjx.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtrtvuyzlv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtiawwgzuk.html

[R69] 生成随机密码
来源：http://hz.jinqigfzy.top/gtspkrwzrp.html

head -c 16 /dev/urandom | base64
来源：http://hz.mhx1999.top/gtymvykthj.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtoqwqgnls.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangkeji.top/gtkvwtbcss.html

[R71] 日期格式化
来源：http://hz.sweek.top/gthyifnxuc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.316326.xyz/gtksehmhhg.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtemsfogja.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gtodolhjsi.html

[R73] 分割大日志
来源：http://hz.shanyushiyangtech.top/gtkfagqcig.html

split -l 1000 big.log part_
来源：http://hz.jlsjyb.cn/gtopgntvgc.html

[R74] 批量重命名
来源：http://hz.daria6918.cn/gtqmgtsckn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gtxnykslcw.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtwimnzneu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuxming.cn/gtubcunidb.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtpodbxhma.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtueeuugvb.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtqpxkjdme.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtrrsevalr.html

[R78] 交互式菜单
来源：http://hz.zhaomingkeji.xyz/gtcxcljeyn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tian-w.cn/gtgkizhqgq.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtcmctwhoq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtfnftuldn.html

[R80] 查看脚本执行耗时
来源：http://hz.guannengcc.top/gtgwhqbxlk.html

time ./run.sh
来源：http://hz.ivvv.top/gttdleodtq.html

================================================================================
来源：http://hz.quarkkingdee.top/gtunmrgbct.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtcexjbxwa.html

================================================================================
来源：http://hz.aibaodan.cn/gtbkhbklto.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtyweblejh.html

#include <stdio.h>
来源：http://hz.cucudq.cn/gtptfrahgu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtxacrapoa.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtmlvykkfl.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtocpbxcci.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtpjmbjcwn.html

int x; scanf("%d", &x);
来源：http://hz.redwolf501.top/gtwdzedghv.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtjsofzgwo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtyhkjevfk.html

[S05] C：字符串长度
来源：http://hz.hnqzz.top/gthqqxfsdq.html

strlen(s)
来源：http://hz.zycfv.cn/gttmpokkyu.html

[S06] C：字符串比较
来源：http://hz.jiagoushi.top/gtibhuprxl.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtkjgvasur.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtcawwiylh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtksuhurhk.html

[S08] C：动态内存分配与释放
来源：http://hz.fzhhl.top/gtlkedgoek.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtjkoxceqc.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtededtoii.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fengsongda.top/gtuamczdjy.html

[S10] C：指针与解引用
来源：http://hz.fzhhl.top/gtrshtrsvd.html

int *p = &a;  *p = 5;
来源：http://hz.jianghu66.top/gtbluxxgto.html

[S11] C：逐行读文件
来源：http://hz.svipenyu.cn/gticfezrdq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtbnjssdmk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gtcjgeynny.html

fclose(f);
来源：http://hz.hnqzz.top/gtackshnfs.html

[S12] C：写文件
来源：http://hz.chenzaomai.com/gtfunzcmwe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shzxlz.cn/gtoajrkrol.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gtvurlluev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dashuyun.cn/gtnqexxgux.html

[S14] C：枚举
来源：http://hz.zhoulong.xyz/gtyuzacedy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guannengcc.top/gtomobdwpq.html

[S15] C：类型转换
来源：http://hz.zdqjudy.top/gtzhrvmwtt.html

(double) a / b
来源：http://hz.jianghu66.top/gtcvtdpxfa.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtvftjgxuw.html

x |= (1 << 3);
来源：http://hz.hnxiangtu.top/gtbbfxuhvo.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtvtpcggdb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cucudq.cn/gtquromhsu.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtxzmureun.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtpavdemue.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtknhltmof.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtrqetthhi.html

[S20] C：二分查找
来源：http://hz.andypj.xyz/gtetdyzkal.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtiquoyhbp.html

[S21] C：字符类别判断
来源：http://hz.jqgfzy.top/gtsjwbquyf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gtoemcqpjw.html

[S22] C：字符串转数字
来源：http://hz.zycfv.cn/gtkdvbxbcv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgufenzy.top/gtmldsbfxb.html

[S23] C：随机数
来源：http://hz.fengsongda.top/gtorpyxqut.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhongyouzk.top/gtocafojyk.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gthhnunvkc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tanke756.top/gtxzfwukom.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtapiyibmr.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtroyszzzi.html

[S26] C：内存清零
来源：http://hz.gaohongyu789.top/gtmsboxedx.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtgrojgvkt.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtzwqzvipd.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtttdbshyc.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtrnqojjgh.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtyuazrsip.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gttctgrhek.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guannengcc.top/gtzwrxdkhi.html

[S30] C：头文件保护
来源：http://hz.jiagoushi.top/gtbglbvwlb.html

#ifndef X_H
来源：http://hz.shzxlz.cn/gtnyrccite.html

#define X_H
来源：http://hz.shzxlz.cn/gtqifqaplj.html

#endif
来源：http://hz.quarkkingdee.top/gthsmwcehm.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gtcjzbzrrh.html

#include <iostream>
来源：http://hz.jinqigfzy.top/gtvtmgvuxg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtbigdmdmy.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtxubryyss.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gtfybgpeyn.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtwsjstlyv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtkjjnpthu.html

[S34] C++：遍历 vector
来源：http://hz.jlsjyb.cn/gtsvbqczqg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gteknjoczs.html

[S35] C++：map
来源：http://hz.316326.xyz/gtusypjdgf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtxlrjzice.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtjaqbhbwk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtndfebydb.html

[S37] C++：set
来源：http://hz.svipenyu.cn/gtkobrshdi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gtwuxnaqzj.html

[S38] C++：排序
来源：http://hz.jlsjyb.cn/gttlouwozd.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gtbfxawqxg.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtvnlsgnon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtpjjqnuag.html

[S40] C++：查找元素
来源：http://hz.yangfankeji.com/gtyuzwbnyk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtyulxvaux.html

[S41] C++：类与构造函数
来源：http://hz.yuanzhike.top/gtozjludeh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigufen.top/gtzocgdwio.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtjtrzxwpm.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtfoqdobmp.html

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gtswmzeplr.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtmpkxdgen.html

[S44] C++：引用传参
来源：http://hz.cqqwz.cn/gtmiplkxra.html

void inc(int &x) { ++x; }
来源：http://hz.hammf.cn/gtvfciucog.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtfzeaazwy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtditfrfzd.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtdbptdlwp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtalbzxgiy.html

[S47] C++：结构化绑定遍历
来源：http://hz.guowangkeji.top/gtgecqxufg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gtfbwgcnhg.html

[S48] C++：逐行读文件
来源：http://hz.xylfe.cn/gtsfzursfr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtodnrkzhr.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gtkhtkbegf.html

[S49] C++：写文件
来源：http://hz.ydjk.org.cn/gtxywayrbl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gttjykwarp.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtafjhtyrs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtoftratvj.html

[S51] C++：显式类型转换
来源：http://hz.ydzc1.top/gtirpyysmq.html

static_cast<double>(a) / b
来源：http://hz.gzhubu.top/gtxjcuzlot.html

[S52] C++：const 与 noexcept
来源：http://hz.chenlongwang.top/gtnqakxjsr.html

int size() const noexcept { return n_; }
来源：http://hz.cashguo.top/gtnxnabzgf.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gtptnqikel.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtroaougjj.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtizelomgx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zdqjudy.top/gtylispvvn.html

[S55] C++：结构化绑定
来源：http://hz.jinghuilouyu.cn/gtabfdlndf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gtolzurfkk.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gttmyuhwba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtfydjvbyy.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtuwrkfuxm.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtsmaavwwc.html

[S58] C++：命名空间
来源：http://hz.pycfn.com/gtxtgrzyxf.html

namespace ns { int f() { return 1; } }
来源：http://hz.xinyue.icu/gtmczhvqow.html

[S59] C++：静态断言
来源：http://hz.jyoumei.cn/gtnleowfdv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gtfhuxuxlw.html

[S60] C++：遍历并删除元素
来源：http://hz.snrcjt.cn/gtwbmlasnt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtckvcjyhc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgbhbmyny.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtahxtlpnm.html

================================================================================
来源：http://hz.yj20258888.top/gtfswepehm.html

[T01] Kotlin：Hello World
来源：http://hz.pengpengdd.cyou/gtrdozkczl.html

println("Hello")
来源：http://hz.zhongyouzk.top/gthisdenpg.html

[T02] Kotlin：变量
来源：http://hz.wangdashe.top/gtcbvnjhqa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtxvpkirsx.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gtbnvkmojm.html

"值: $b"
来源：http://hz.yuxming.cn/gtfnsqmpqf.html

[T04] Kotlin：空安全
来源：http://hz.yvedp.cn/gtzxnazswe.html

val n: String? = null;  n?.length
来源：http://hz.wangdashe.top/gtejaafkpk.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtnvizgzag.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnxiangtu.top/gtfqxfxloy.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtwklyqzbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangkeji.top/gtipozbtte.html

[T07] Kotlin：集合过滤
来源：http://hz.quarkkingdee.top/gtafobczzf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cdnleiting.top/gtikekeizh.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gtyxtzfner.html

data class User(val name: String, val age: Int)
来源：http://hz.fzhhl.top/gtnvhoimfy.html


<!-- 参考信息 -->