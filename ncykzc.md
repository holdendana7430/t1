代发 wailian999

R. Bash 专题
来源：http://hz.yuanzhike.top/gtckbpabsd.html

================================================================================
来源：http://hz.snrcjt.cn/gtbnyghjvn.html

[R01] shebang 与严格模式
来源：http://hz.cucudq.cn/gthxvzsojf.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtfjhmushs.html

set -euo pipefail
来源：http://hz.pycfn.com/gtvdkkmyud.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtkcezyjbb.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtdgxlmlbs.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtvawflvig.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtzbdiczui.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtviqgrhtp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtyvjaqatz.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtlplxjuoj.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtzngyglyr.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtmgjivscl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtfoixnswc.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtsitelnjy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtuakpembf.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtwifyuspc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gttcfogomk.html

[R09] 字符串比较
来源：http://hz.zhoulong.xyz/gtouetwdut.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtsvwrfqck.html

[R10] 正则匹配
来源：http://hz.xinyue.icu/gtjjwlproa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtfeqslngx.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtcqasjvrg.html

case "$1" in
来源：http://hz.pycfn.com/gtstakfgfp.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtmmpzpsly.html

stop)  echo "停止" ;;
来源：http://hz.ybcxt.top/gtljvatvik.html

*)     echo "未知命令" ;;
来源：http://hz.yuanzhike.top/gtqjwxdvkx.html

esac
来源：http://hz.yongpay.top/gtmfgikcag.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gthgqmjkay.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gthesxkdly.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtuyrrndkl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtkudkyxla.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtiqcxlylb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtzchdrrkm.html

[R15] while 逐行读文件
来源：http://hz.xinyue.icu/gtdabpyyax.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.haohaochexian.top/gtgaadkywv.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtxihcsgcj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtbtvdderh.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gtdxiiisnz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtqforegmt.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gtdfdjfhkw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnxiangtu.top/gtqtgmfedo.html

[R19] 数组长度
来源：http://hz.snrcjt.cn/gtmddrglsa.html

echo "${#arr[@]}"
来源：http://hz.ydjk.org.cn/gtrjsyfipy.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtcjciynji.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fzhhl.top/gtnjerpxsn.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtccsckjri.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtstritxyk.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtytphisjf.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtnvbdaysc.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtgjxurunx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtcthqbpjo.html

[R24] 大小写转换
来源：http://hz.hysaishi.cn/gtmskbljlj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shzxlz.cn/gtsiegslrc.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtlntychnk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtdbvvwybr.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtbbhqadyh.html

now=$(date +%F); echo "$now"
来源：http://hz.shuidangran.top/gteljrferp.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtpydhklxx.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtalukwkqu.html

[R28] 浮点运算
来源：http://hz.zhoulong.xyz/gtapsgzmrf.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtulzarbdi.html

[R29] 定义函数
来源：http://hz.gotoacloud.top/gtqqvcenac.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtudkxrumv.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gttzmgygep.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gtdrmaecmz.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtuggzppom.html

f() { local x=1; echo "$x"; }
来源：http://hz.hywenlv.cn/gtxubaoljx.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtajeapizz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtmdcejhwv.html

[R33] 捕获错误并提示行号
来源：http://hz.yuanzhike.top/gtqhrxrcwr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtdwtktyzq.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtwewvhoto.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtuiomrloq.html

[R35] 后台执行并等待
来源：http://hz.hnqzz.top/gtwqtsghsa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cdnleiting.top/gtjujmmmxk.html

[R36] 并发执行多个任务
来源：http://hz.ydjk.org.cn/gtdomuoull.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtakaforjk.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtsqyfwljk.html

files=$(ls -1)
来源：http://hz.hnqzz.top/gtctnimbvc.html

[R38] 管道串联
来源：http://hz.shanyushiyangkeji.top/gtcxhsdcpt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtzoemucyh.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gttwojgiqh.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtfczszqah.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtqwxoyvlw.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtugpwghja.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtefsazxxg.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtoyakopoh.html

[R42] 输入重定向
来源：http://hz.jinghuilouyu.cn/gtulgadscw.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtebolydks.html

[R43] 按名字查找文件
来源：http://hz.yj20258888.top/gtskiahiyh.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtscvxlsho.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtamdsgotp.html

find . -mtime -7 -type f
来源：http://hz.nwbrower.top/gtvxmxpwhv.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtugglgmdn.html

find . -name "*.tmp" -delete
来源：http://hz.hysaishi.cn/gtzwyhjxch.html

[R46] 递归替换文件内容
来源：http://hz.chenjidiqi.icu/gttderetda.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gzhubu.top/gtuhquobgj.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gtnxzbesxr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gtcxrppovs.html

[R48] awk 取指定列
来源：http://hz.xinyue.icu/gtyfylkhcu.html

awk '{print $1, $3}' a.txt
来源：http://hz.yueranfly.top/gtwriqiivt.html

[R49] awk 带条件
来源：http://hz.zhiwuduotai.top/gtxhsfitbs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cashguo.top/gtyilwyrjt.html

[R50] awk 求和
来源：http://hz.jlsjyb.cn/gtvtzbilpk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtukemknqt.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gthnufmvvf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtypvvhlwr.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtzpdnsllu.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtmnzynlvk.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtrsbgnzre.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtkbbmalfw.html

[R54] 比较两个文件
来源：http://hz.gaohongyu789.top/gtfstoyyqb.html

diff a.txt b.txt
来源：http://hz.sufxvd.cn/gtthuvatua.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtmhpyutub.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gttfiivvnb.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gtcjtgovod.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gtskhleyop.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gtlzkjtrct.html

ssh user@host 'uptime'
来源：http://hz.zhiwuduotai.top/gtszbxxmot.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtjdnamuwn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtzxpobbvy.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtkopnnajc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sufxvd.cn/gtgqvxdvvk.html

[R60] 只看 HTTP 状态码
来源：http://hz.yvedp.cn/gtpqtgiajw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gtlfuvfjtk.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gttjqmcvih.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtchcncfiq.html

[R62] 找最占空间的文件
来源：http://hz.tianlin.xyz/gtjnfqysgb.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtkhkrtdrj.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtshytojka.html

free -h;  ps aux | grep nginx
来源：http://hz.0kj1m.cn/gtjnytdvsf.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gttwxudgix.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtclikqban.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangkeji.top/gtniyrvovj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xinyue.icu/gtexgrvzup.html

[R66] 定时任务
来源：http://hz.gaohongyu789.top/gtqzgtggpq.html

crontab -e;  crontab -l
来源：http://hz.zhixingplan.top/gtaltjhhnq.html

[R67] 生成随机十六进制串
来源：http://hz.jinghuilouyu.cn/gtuatyvxgc.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtwlkomohc.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gtltxytdmu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gtfurqjwes.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtcaaktcsn.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtzsjechmm.html

[R70] 时间戳与互转
来源：http://hz.yvedp.cn/gtsikqqzpn.html

date +%s;  date -d @1700000000
来源：http://hz.hfpthk.cn/gtippcxiix.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtkhbxgmur.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gtplxpszzh.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtwavsuisj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtlxhkhysf.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtinxkmxwt.html

split -l 1000 big.log part_
来源：http://hz.yuxming.cn/gtymkikxpn.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gthmujvonj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fzhhl.top/gtlanmgaah.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtyoeqiakw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtrtirdkkr.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtuvbgnjbt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtvbcsnoak.html

[R77] 读取用户输入
来源：http://hz.hysaishi.cn/gtkxipkqqr.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtdajpdhfi.html

[R78] 交互式菜单
来源：http://hz.chenjidiqi.icu/gtetfgvfev.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.snrcjt.cn/gtttdhsttl.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtebrwwfqq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj202588.top/gtnvdebjbw.html

[R80] 查看脚本执行耗时
来源：http://hz.0kj1m.cn/gtqcrevndu.html

time ./run.sh
来源：http://hz.0kj1m.cn/gtkfvhyyjr.html

================================================================================
来源：http://hz.xuanzx.com/gtpdbvfpmi.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtczqaduuf.html

================================================================================
来源：http://hz.yangfankeji.com/gtfobwdygt.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gtwwicxwqj.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtwzfmzhwx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtfyacupru.html

[S02] C：变量与格式化输出
来源：http://hz.hfpthk.cn/gtczodiqtw.html

int a = 10; printf("%d\n", a);
来源：http://hz.gaohongyu789.top/gtxrmbfgbk.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtpueawkst.html

int x; scanf("%d", &x);
来源：http://hz.wangdashe.top/gtrnwidnad.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtmzrisjwo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtoewfrpqt.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtgsnndcnw.html

strlen(s)
来源：http://hz.aibaodan.cn/gtdbfcpsbl.html

[S06] C：字符串比较
来源：http://hz.guannengcc.top/gtbxygcrgb.html

strcmp(a, b) == 0
来源：http://hz.jinqigufen.top/gtwhszmrzc.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtrljjkkyp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.birdmap.top/gteizoqtty.html

[S08] C：动态内存分配与释放
来源：http://hz.cqqwz.cn/gthyjibtnn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtvutsfoym.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtauflfjhr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hfpthk.cn/gtdrbpwxam.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtczwvrcqy.html

int *p = &a;  *p = 5;
来源：http://hz.redwolf501.top/gtnpbcfpsc.html

[S11] C：逐行读文件
来源：http://hz.tianlin.xyz/gtirrmoqdn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydjk.org.cn/gtykdappgg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gttxubwmqx.html

fclose(f);
来源：http://hz.ehwqpu.com/gtrravtvfp.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtugipeypt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.316326.xyz/gthxvhnjkt.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtnjlaksgn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigfzy.top/gtjkfwhstl.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtetjdwfha.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtaybmvmik.html

[S15] C：类型转换
来源：http://hz.jqgfzy.top/gtaseqavxm.html

(double) a / b
来源：http://hz.cdnleiting.top/gtpgsckjqx.html

[S16] C：位操作置位
来源：http://hz.jinqigfzy.top/gtgzdeyvum.html

x |= (1 << 3);
来源：http://hz.shuidangran.top/gtqqjisbfw.html

[S17] C：安全拼接字符串
来源：http://hz.cheryme.top/gtwddlcxwu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtoczrvebs.html

[S18] C：命令行参数
来源：http://hz.sxryk.cn/gtxgncideo.html

int main(int argc, char **argv)
来源：http://hz.xingfuxueyuan.xyz/gtdjrluese.html

[S19] C：快速排序
来源：http://hz.shanyushiyangkeji.top/gtzjuvuqby.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtyrufbixu.html

[S20] C：二分查找
来源：http://hz.yueranfly.top/gtmfkeykyb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtirdciira.html

[S21] C：字符类别判断
来源：http://hz.ydjk.org.cn/gtlwvrogxt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxuanxn.top/gtncjcocux.html

[S22] C：字符串转数字
来源：http://hz.hnxiangtu.top/gtpxmbhyli.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtgyvrrncu.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtgvdeenhy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtprfdotbp.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtlrvludng.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.316326.xyz/gtncwebhyx.html

[S25] C：内存拷贝
来源：http://hz.nanxuanxn.top/gtpxgyxhur.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtcunqwlkh.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtqsasljgu.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gttvpmyjtn.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtovewaoeb.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtwtrlzaul.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtqpmllrfo.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtnmimuyda.html

[S29] C：变参函数
来源：http://hz.gogol.net.cn/gtgowdqegu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtcdqoqtbm.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtpcwrgbwc.html

#ifndef X_H
来源：http://hz.yongpay.top/gttarwaamo.html

#define X_H
来源：http://hz.aizwys.cn/gtagsfrjcg.html

#endif
来源：http://hz.shanyushiyangtech.top/gtkfgjuswd.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtrspnbjmm.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtxghhnrpy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shzxlz.cn/gtykoqbhgs.html

[S32] C++：字符串
来源：http://hz.pycfn.com/gtceuszbbr.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtiswyjqfb.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtjqjyqamm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gttbwhebee.html

[S34] C++：遍历 vector
来源：http://hz.xuanzx.com/gtfaqxrwfm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yonumen.top/gtdgxetyui.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtbafyykle.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtjyzxammv.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtyjdtdspq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtfiauwxcw.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtdqujagca.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gtnwszitgw.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gtxzidvrjv.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtlmilnrxj.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigfzy.top/gttjkkepgq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtmteqnynv.html

[S40] C++：查找元素
来源：http://hz.yvedp.cn/gtlrcqhbtz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gttpbcwqrj.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtknuyfbjw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtkqyrbvfr.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigufen.top/gtckrvmmbu.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtsjsiugst.html

[S43] C++：智能指针
来源：http://hz.birdmap.top/gtzuzcakdd.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtemgogmsu.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtligurouj.html

void inc(int &x) { ++x; }
来源：http://hz.aibaodan.cn/gtaisruudr.html

[S45] C++：lambda
来源：http://hz.chenzaomai.com/gtzcwovhhz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtbyjalzoo.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtnswvfctc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangdashe.top/gtzlklqkpc.html

[S47] C++：结构化绑定遍历
来源：http://hz.cdnleiting.top/gtddlffnbn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtfhmvzrbh.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtdvdzrcpm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtpyuxtvts.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtkkttpjrt.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtpwkxskoo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhiwuduotai.top/gtbwpntwwi.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtcbishxrz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gtnghjyehn.html

[S51] C++：显式类型转换
来源：http://hz.gzhubu.top/gtoulbfeur.html

static_cast<double>(a) / b
来源：http://hz.ehwqpu.com/gtfjweokxl.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gtxraaowax.html

int size() const noexcept { return n_; }
来源：http://hz.yueranfly.top/gturneoitj.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtmszawbrp.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtotswezbq.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtsyozgyrv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtcepcnrgw.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtcztjtxsl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtllmggrby.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtqmgngyuc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtmumyjrlk.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gtoenjbvwb.html

constexpr int N = 10;
来源：http://hz.sufxvd.cn/gtjmszhrbc.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtzcluzcej.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnxiangtu.top/gtpvruompl.html

[S59] C++：静态断言
来源：http://hz.chenlongwang.top/gtehoyixlr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtbgjmkqou.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtykkoednn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gtjgjqqeik.html

================================================================================
来源：http://hz.bjfxy.top/gthgbwmipf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtpuxllazw.html

================================================================================
来源：http://hz.hywenlv.cn/gtcauammgv.html


<!-- 参考信息 -->