代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yangfankeji.com/gtjrgqvxij.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtbwlkdepf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxinkj.top/gtgfamogaf.html

[R09] 字符串比较
来源：http://hz.mhx1999.top/gtgrdnlmxi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtlcjnqtxv.html

[R10] 正则匹配
来源：http://hz.shanyushiyangkeji.top/gtliywhlxr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yanxiufei.cn/gtykywmmdj.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtgxgsivmr.html

case "$1" in
来源：http://hz.316326.xyz/gttpkjipss.html

start) echo "启动" ;;
来源：http://hz.gotoacloud.top/gtqanvqgmq.html

stop)  echo "停止" ;;
来源：http://hz.9152youxi.cn/gtggsooxkj.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gthoahvqpo.html

esac
来源：http://hz.yj202588.top/gtzecapdqi.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtdlpfrdio.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtocqnwofg.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtvvxnzpwg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gtanyemkvt.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gtefrptrct.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtanthlqrf.html

[R15] while 逐行读文件
来源：http://hz.redwolf501.top/gtvfbwrbio.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gtfypgbgqf.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtscgljqcf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtakwclymy.html

[R17] 数组定义与取值
来源：http://hz.zhoulong.xyz/gtzvxtlssr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gtjqbdfjcl.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtazzrumsr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.kuanghao11.cn/gtkydnirvh.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtkgfbkuuk.html

echo "${#arr[@]}"
来源：http://hz.yanxiufei.cn/gtrjywqjto.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtonfknigj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtpkkmryce.html

[R21] 字符串长度
来源：http://hz.hywenlv.cn/gtxsytfdoq.html

echo "${#s}"
来源：http://hz.jiagoushi.top/gtzhagcntp.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtmcwdbfyd.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtzhobopcs.html

[R23] 字符串替换
来源：http://hz.sysykeji.top/gtucbqqycn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.quarkkingdee.top/gtorczuyhj.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gtxlpvqzzm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtcnidtzbh.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydzc1.top/gthptvmvbp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtjsqnnulu.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtqhdebxam.html

now=$(date +%F); echo "$now"
来源：http://hz.c1oappe.top/gtmxxuzxoo.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gtdwulzkio.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtwtyigict.html

[R28] 浮点运算
来源：http://hz.jinqigufen.top/gtwgtuvjjf.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtdfqdozfh.html

[R29] 定义函数
来源：http://hz.shanyushiyangtech.top/gtfcighvli.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnxiangtu.top/gtvhmfxcwh.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtjuldgduu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtsfpkxqnq.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtdfeyboux.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtsnnxyipb.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtchkzfxqp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtjmtaqpzf.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtcnvtimjl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtgfurdvds.html

[R34] 退出时清理
来源：http://hz.chenjidiqi.icu/gtqhhpryvc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtoultgojx.html

[R35] 后台执行并等待
来源：http://hz.cheryme.top/gtwqdwpnce.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gtwnevcdua.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtdixeoekv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtmxjlnrwh.html

[R37] 把输出赋给变量
来源：http://hz.ppjwa.cn/gtfrkevaes.html

files=$(ls -1)
来源：http://hz.jinqigfzy.top/gtiqxksohr.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtgkodxztc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtgfowvdzx.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtwrgdvacn.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtyfojtiiq.html

[R40] 追加写日志
来源：http://hz.xylfe.cn/gtvtbtxqks.html

echo "log" >> out.log
来源：http://hz.mhx1999.top/gtgqmblsym.html

[R41] 丢弃输出
来源：http://hz.smart0.xyz/gtltwzjuta.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gthmbdpnpj.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtmpabgqyw.html

wc -l < a.txt
来源：http://hz.cdnleiting.top/gtmichoxtm.html

[R43] 按名字查找文件
来源：http://hz.daria6918.cn/gtjfrdoodv.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gttpbjlqnp.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtzsnqejgk.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtiwghjxox.html

[R45] 批量删除
来源：http://hz.gogol.net.cn/gtofyhmpur.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtguhrzgjp.html

[R46] 递归替换文件内容
来源：http://hz.ydzc1.top/gtkrhnntgz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtyrktdcll.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gthpyfaxsr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.havefunace.top/gtkpbiwgjt.html

[R48] awk 取指定列
来源：http://hz.aizwys.cn/gtozbovuvw.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtahmwpxaq.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtawlgfrdu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtwthxhrso.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtopwzljqs.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtgmpnbxwy.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gteyshhyjx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gttvlxnkqr.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtucpkvkzu.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gtogfbagxj.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtputzxtut.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhongyouzk.top/gtjvhpraol.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtbdirfowj.html

diff a.txt b.txt
来源：http://hz.fzhhl.top/gtghygqjml.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtftoyoyss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.316326.xyz/gtpwzbogle.html

[R56] 远程拷贝
来源：http://hz.ppjwa.cn/gtkotgyifv.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtgxfttofv.html

[R57] 远程执行命令
来源：http://hz.yanxiufei.cn/gteenbkqfw.html

ssh user@host 'uptime'
来源：http://hz.hysaishi.cn/gtubsmdiyr.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtncjcnabf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hammf.cn/gthvflaxmj.html

[R59] 发 POST JSON
来源：http://hz.nanxinkj.top/gtwqgqgvst.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.havefunace.top/gtygsatodv.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtduyigyhz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtmyfwatxt.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gtselqizus.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gthrpfnrec.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtpubgjzbw.html

du -ah . | sort -rh | head -10
来源：http://hz.dianchejie.cn/gtgfxsptvb.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gtnogmuhbd.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtmnsrzyem.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtjkzzlzju.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gtxtjhcnjx.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtalimmcph.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtsryqeiiu.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtmzymiles.html

crontab -e;  crontab -l
来源：http://hz.yuanzhike.top/gtametebat.html

[R67] 生成随机十六进制串
来源：http://hz.yuxming.cn/gtjgzpvwlg.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gthvipyjgv.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtoraxtehw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtanxegexv.html

[R69] 生成随机密码
来源：http://hz.hnxiangtu.top/gtppvpfnyb.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtciuuponr.html

[R70] 时间戳与互转
来源：http://hz.jianghu66.top/gtsxxumhdl.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gtpvbslzgc.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtwzpjduye.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gtjdzsxmji.html

[R72] 等待端口就绪
来源：http://hz.yuxming.cn/gtzqzbjijw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtbeacfybx.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtdxazuxop.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtahuworjm.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtrzokvbko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtrtnjkluo.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gthjvssufb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtdgnoiuwe.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtierpmnhu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtxkjlrmky.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gttfiqqhrt.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtgvpkflcy.html

[R78] 交互式菜单
来源：http://hz.sufxvd.cn/gtsahffyed.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhijiandao.cn/gtcdlqpwum.html

[R79] 解析命令行选项
来源：http://hz.birdmap.top/gtvuyaabny.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtdzinxbvi.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtncptfmbg.html

time ./run.sh
来源：http://hz.pengpengdd.cyou/gtkpeemuzi.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtonzfrwgn.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtloyjiaav.html

================================================================================
来源：http://hz.yuanzhike.top/gtyjwwanfo.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtqmagvifa.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtdubjemco.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtcavpeyaf.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtpcglhtlm.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuetiantiany.cn/gtvifdkoab.html

[S03] C：读入整数
来源：http://hz.nwbrower.top/gtnfwlxwln.html

int x; scanf("%d", &x);
来源：http://hz.9152youxi.cn/gtunugviuh.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtnwdnzzfe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cucudq.cn/gtbebeaurb.html

[S05] C：字符串长度
来源：http://hz.fzhhl.top/gtxegznyud.html

strlen(s)
来源：http://hz.tanke756.top/gtcathuoet.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtsxcvitcp.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtlyvbeeno.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gtiongycpr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtudavfjws.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigufen.top/gtfqgjkhtw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtjilkmmfd.html

[S09] C：结构体定义与初始化
来源：http://hz.yuxming.cn/gtdoalxxrt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gaohongyu789.top/gtdmthoiug.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtqdxksiqp.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtvrqkvtrd.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtormyhsph.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnxiangtu.top/gtzbwczbef.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtggfejotv.html

fclose(f);
来源：http://hz.shuidangran.top/gtyzuvfhjk.html

[S12] C：写文件
来源：http://hz.ivvv.top/gtzxcugkzv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtengtifxg.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtxhyemxdz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtjxihfyan.html

[S14] C：枚举
来源：http://hz.tianlin.xyz/gtcpfzghlr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jyoumei.cn/gtktrrosjw.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtbzljartc.html

(double) a / b
来源：http://hz.jqgfzy.top/gtmhnkfpjc.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtdcbxsotc.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gtkfyoiork.html

[S17] C：安全拼接字符串
来源：http://hz.dashuyun.cn/gttaisztoy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtsimygfad.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtrgfjdckg.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtrrglwsle.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtsoxsvles.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtcvvalkmp.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtxqaagpmm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtfnfftxpc.html

[S21] C：字符类别判断
来源：http://hz.ydjk.org.cn/gtpdkshznb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cucudq.cn/gtvfmldwmk.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gtzzfrbbvr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sufxvd.cn/gtiyykkykl.html

[S23] C：随机数
来源：http://hz.aizwys.cn/gttvbijgbv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangtech.top/gtvmjfqwva.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtynnwavbr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.0kj1m.cn/gtxkegbsrm.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gthnnmnrva.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtlpditcsm.html

[S26] C：内存清零
来源：http://hz.tanke756.top/gtuayrzknu.html

memset(a, 0, sizeof a);
来源：http://hz.c1oappe.top/gtvxnijhck.html

[S27] C：定义常量
来源：http://hz.jinyuanbaomall.cn/gtimvcwdsn.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtppbsrxcd.html

[S28] C：静态变量
来源：http://hz.yj202588.top/gtfmqvpffp.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtjwulkizo.html

[S29] C：变参函数
来源：http://hz.c1oappe.top/gttewvkfhc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.316326.xyz/gtqdruotvv.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gtqpidtdhj.html

#ifndef X_H
来源：http://hz.zhiwuduotai.top/gtimextknr.html

#define X_H
来源：http://hz.quarkkingdee.top/gtuphncbov.html

#endif
来源：http://hz.jqgufenzy.top/gtjylkjjxc.html

[S31] C++：Hello World
来源：http://hz.shangyingyoupin.top/gtwfoxvdfx.html

#include <iostream>
来源：http://hz.zhaomingkeji.xyz/gtswovypty.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daxiang520.top/gtiaidkuzl.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtdqjvkpeq.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtaveygizb.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtqxsuaqdx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.0kj1m.cn/gtxjbfdoin.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gtlmicxiul.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtxmbnsxfv.html

[S35] C++：map
来源：http://hz.tanke756.top/gtghcuhtyb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtgemmqlgz.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtcprrsvpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtgczsruik.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtkmbuleae.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtnjjguezi.html

[S38] C++：排序
来源：http://hz.zhengqikj.top/gtovswvilw.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtpbzxgonl.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtpifpiqyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtdzxdlsks.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtwfcqsoew.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhongyouzk.top/gtriqmawrt.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtaiksxvfd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtbaqxfcjd.html

[S42] C++：继承与虚函数
来源：http://hz.cucudq.cn/gteckgdqeq.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtypkequqk.html

[S43] C++：智能指针
来源：http://hz.gaohongyu789.top/gtuanxmwoy.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtuxdpgxss.html

[S44] C++：引用传参
来源：http://hz.tianlin.xyz/gtbvuaptrg.html

void inc(int &x) { ++x; }
来源：http://hz.aibaodan.cn/gtdpewrdmr.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gtwrfxumyj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtprjuompc.html

[S46] C++：函数模板
来源：http://hz.xingfuxueyuan.xyz/gtvfnfnhvh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.mhx1999.top/gtfwecxhhc.html

[S47] C++：结构化绑定遍历
来源：http://hz.fzhhl.top/gtnvhfwflo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj202588.top/gtlzyntswz.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtcpiadusi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cashguo.top/gtzkuoacqp.html

while (std::getline(in, line)) { }
来源：http://hz.tianlin.xyz/gtwukxejvb.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtcboimqtj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtkghvaqcj.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtjzyaccsk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtejzcscrw.html

[S51] C++：显式类型转换
来源：http://hz.yvedp.cn/gtigwglqen.html

static_cast<double>(a) / b
来源：http://hz.gotoacloud.top/gtvmzoiodv.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtpkapjkou.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtthmkzund.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtoljehzbn.html

std::vector<int> w = std::move(v);
来源：http://hz.tianlin.xyz/gtskciwgqr.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gthttyhvcm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.havefunace.top/gtiuvssprz.html

[S55] C++：结构化绑定
来源：http://hz.zhiwuduotai.top/gtodhjrmen.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtcsvftelp.html

[S56] C++：optional
来源：http://hz.shuidangran.top/gtzykhrkxr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtdlyxkinw.html

[S57] C++：编译期常量
来源：http://hz.yangfankeji.com/gtnhayxrve.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtqebelipt.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtaaaqkrpu.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtuyhvuwny.html

[S59] C++：静态断言
来源：http://hz.kuanghao11.cn/gtgnqvqsbk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.snrcjt.cn/gtbfatljpr.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtbkbygxjj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtlsmecwvb.html

================================================================================
来源：http://hz.jiagoushi.top/gtrmhnxlix.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtjcndaebv.html

================================================================================
来源：http://hz.cucudq.cn/gtvgtuzciu.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtdmxzdnxs.html

println("Hello")
来源：http://hz.guannengcc.top/gtvfesmekf.html

[T02] Kotlin：变量
来源：http://hz.dashuyun.cn/gtnimqxeqv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.iojbl.cn/gtmyuikupp.html

[T03] Kotlin：字符串模板
来源：http://hz.guowangkeji.top/gtdxudzkzj.html

"值: $b"
来源：http://hz.mhx1999.top/gtlqxmtdwb.html

[T04] Kotlin：空安全
来源：http://hz.hongshengwenyu.top/gtwikhgsfu.html

val n: String? = null;  n?.length
来源：http://hz.wangshuangyany.cn/gtfjqisres.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtjeaqxpid.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gotoacloud.top/gtddpszmps.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gthiifvkbe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fengsongda.top/gtuudbygqk.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258888.top/gtecngjlbc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtvuzotsfy.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gthtvxtezf.html

data class User(val name: String, val age: Int)
来源：http://hz.shzxlz.cn/gthwdxluif.html


<!-- 参考信息 -->