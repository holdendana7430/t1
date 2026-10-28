代发 wailian999

esac
来源：http://hz.wangshuangyany.cn/gtegxybgls.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtbjwcoerp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tian-w.cn/gtwkelwgvc.html

[R13] for 计数循环
来源：http://hz.hysaishi.cn/gtzympebsy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtsvlqkjsm.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtsoctbqxz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtfqyrsjng.html

[R15] while 逐行读文件
来源：http://hz.zhijiandao.cn/gtgzmbrtbg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yonumen.top/gtqvhmsecs.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtifpopgrf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gthlodqzfg.html

[R17] 数组定义与取值
来源：http://hz.xziqi.cn/gtlfsakfaq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtlnstnorr.html

[R18] 遍历数组
来源：http://hz.jinqigufen.top/gtrzsqqjlp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtwidjebgm.html

[R19] 数组长度
来源：http://hz.sweek.top/gtubykmvct.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gtxmedcnjc.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangtech.top/gtteczcudb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtmxvrejjt.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtxzsubebc.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtucwuauqc.html

[R22] 截取子串
来源：http://hz.cucudq.cn/gtwudnvcth.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtwsrepdce.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtvmcfxubl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtjmxwycre.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtzeimffwp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ivvv.top/gticwrtnyn.html

[R25] 去后缀 / 去前缀
来源：http://hz.svipenyu.cn/gtahxocxyl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtjmvsbxis.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtudyfwzss.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigufen.top/gtxidtbutc.html

[R27] 算术展开
来源：http://hz.xinyue.icu/gthaecsouz.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtcplagoht.html

[R28] 浮点运算
来源：http://hz.xuetiantiany.cn/gtxlgdgzsh.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtdflqvwic.html

[R29] 定义函数
来源：http://hz.chenjidiqi.icu/gtndyjvufl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtycmtuavb.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gttneujlvz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtfliqmxdo.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gteclfjenc.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gtzxzixdek.html

[R32] 参数个数校验
来源：http://hz.yuxming.cn/gtenrylmtu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aizwys.cn/gtwcdzsefx.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtjnsurbzz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtqksvgqmy.html

[R34] 退出时清理
来源：http://hz.cheryme.top/gtydlyxnpk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtdmcnhxjj.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtptsuyfvh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tianlin.xyz/gtbejttbuv.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtwdeddmws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuxming.cn/gtjrzseszh.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gtjuiiovtd.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtrlsoeqih.html

[R38] 管道串联
来源：http://hz.sweek.top/gtwfkmjdkt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gtxyhphewd.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtqyqckfjo.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtoqipobig.html

[R40] 追加写日志
来源：http://hz.nanxinkj.top/gtwqvmqfnz.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtltevefmr.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtemuozrih.html

cmd >/dev/null 2>&1
来源：http://hz.gogol.net.cn/gtszrbjooz.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gtkmgaxarn.html

wc -l < a.txt
来源：http://hz.sweek.top/gtnolmxkle.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gtkttxdjhi.html

find . -name "*.log" -type f
来源：http://hz.iojbl.cn/gtyxaonnii.html

[R44] 按修改时间查找
来源：http://hz.cheryme.top/gthcjrzpvi.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtjjrhbosf.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gttcdgiplk.html

find . -name "*.tmp" -delete
来源：http://hz.fengsongda.top/gtfiduislq.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtamevefkt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtrapxkogy.html

[R47] sed 单行替换
来源：http://hz.ybcxt.top/gtdoxdntnw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tanke756.top/gtccnvyftq.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtuzivsiaq.html

awk '{print $1, $3}' a.txt
来源：http://hz.quarkkingdee.top/gtyezjfbtj.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gtkokgugys.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgufenzy.top/gtyjzjalvg.html

[R50] awk 求和
来源：http://hz.yj20258.top/gtlsehoxcf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgufenzy.top/gtpohbyshk.html

[R51] 排序去重取前几
来源：http://hz.shangyingyoupin.top/gthtxmuake.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sweek.top/gtjukewvzm.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtfybagjiw.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtfmnlifww.html

[R53] 查看文件头与实时尾
来源：http://hz.hfpthk.cn/gtyhlthatj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtkneyadxa.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gthpitygcp.html

diff a.txt b.txt
来源：http://hz.havefunace.top/gtbobxpnmd.html

[R55] 压缩与解压
来源：http://hz.daria6918.cn/gtuptpgloe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtttofhfgo.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtxmlctwnx.html

scp file user@host:/path/
来源：http://hz.jinqigfzy.top/gthbowhnuf.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gttpuztdqs.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gttmacyiwr.html

[R58] 下载文件
来源：http://hz.gogol.net.cn/gtzwrvqbio.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtupsywlnv.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtrxlhdqoh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtfzqogomc.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtwpnlmcbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtvrmaedxf.html

[R61] 磁盘占用
来源：http://hz.meibo888.top/gtsveardil.html

df -h;  du -sh *
来源：http://hz.jinyuanbaomall.cn/gtzvtjvdei.html

[R62] 找最占空间的文件
来源：http://hz.dashuyun.cn/gthxvbqvqb.html

du -ah . | sort -rh | head -10
来源：http://hz.hnxiangtu.top/gtmvitsbke.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtqowyobcm.html

free -h;  ps aux | grep nginx
来源：http://hz.feifeiyinyue.top/gtrvkaofjw.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtnokteoyg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtcwehnlcj.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtwzolcdvv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yanxiufei.cn/gtdejvrfsl.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtwkjcxkso.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtzlqyvdzy.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtknbamzhm.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtecsnfkhe.html

[R68] 计算文件校验值
来源：http://hz.havefunace.top/gtwvoshhwy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtuyfavpgp.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtxtsmpruu.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtxoxumkdh.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtgqogqlau.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtpzefisyj.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtkdxthjnf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shuidangran.top/gtbktlfpvh.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtbafxxlxd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gotoacloud.top/gttqgzngnl.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtbrvforna.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gtduwibczf.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtojmrgslj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtuuiqczcd.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtsfirmsdq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.meibo888.top/gtvqtjbbde.html

[R76] 使用临时文件
来源：http://hz.shuidangran.top/gtlzrzrurs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtbvioklxa.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtstnsrhoo.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gteysnezxr.html

[R78] 交互式菜单
来源：http://hz.zycfv.cn/gtoboyvyxz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtuprxaybv.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gthcvyqgdg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtomwymvtz.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgfzy.top/gtykkppvwv.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtvhzsbzkx.html

================================================================================
来源：http://hz.daxiang520.top/gtvdicqyqx.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gthkshaijb.html

================================================================================
来源：http://hz.ivvv.top/gtplkeshvs.html

[S01] C：Hello World
来源：http://hz.dianchejie.cn/gtslxspmzi.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtssmdofls.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtekdxhobi.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gthyosived.html

int a = 10; printf("%d\n", a);
来源：http://hz.zycfv.cn/gtruqsnguh.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtrcegqioa.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtlnsupepp.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtakvrcivz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtoymradja.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtcqyjjorr.html

strlen(s)
来源：http://hz.jlsjyb.cn/gtzuukqwby.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtmnkooumz.html

strcmp(a, b) == 0
来源：http://hz.tian-w.cn/gthtetuowv.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtztybusnt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtbgwtfsyj.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtaecmfikq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.meibo888.top/gtwqcfzwli.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gtkuiwumar.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtdfeqelbz.html

[S10] C：指针与解引用
来源：http://hz.jinqigufen.top/gtaxnvsefv.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtoaksqhhr.html

[S11] C：逐行读文件
来源：http://hz.fzhhl.top/gtgsnszujn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gtwdpijicx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtcekpswox.html

fclose(f);
来源：http://hz.zhoulong.xyz/gtummjjvvt.html

[S12] C：写文件
来源：http://hz.yvedp.cn/gttutmjfhs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtquijqfoe.html

[S13] C：宏定义
来源：http://hz.zhoulong.xyz/gtezfiiaqk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cucudq.cn/gtrzpgjucj.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gtobjehzjd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gtwdyrbhgg.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gtihglgsod.html

(double) a / b
来源：http://hz.gotoacloud.top/gtanyswzkt.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtzlxtrbru.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtvojtyrwj.html

[S17] C：安全拼接字符串
来源：http://hz.yuanzhike.top/gtaaxozeqz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtdpwsdvys.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtcvbosjkd.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtclxcwxsl.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtgpoobvhn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtslaeziqk.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtelqawqef.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtarzwailm.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtsnlbvpof.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuxming.cn/gtftswazfb.html

[S22] C：字符串转数字
来源：http://hz.guowangkeji.top/gtdclujkoi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtixwxnrmc.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtdwnoknim.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258.top/gtityvkzrn.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtkasscjpv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtolakhusw.html

[S25] C：内存拷贝
来源：http://hz.nwbrower.top/gtssxctxed.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gtpmixvxnj.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gteuvrdswa.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtkysdnpoq.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtpxquikim.html

const double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtsyhgmqpc.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtymgslqvt.html

static int counter = 0;
来源：http://hz.hnxiangtu.top/gtgkzfzexf.html

[S29] C：变参函数
来源：http://hz.hnxiangtu.top/gtlawmwqsx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtqewrcjpd.html

[S30] C：头文件保护
来源：http://hz.gaohongyu789.top/gtjorhcpta.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtttyhifjh.html

#define X_H
来源：http://hz.jinqigufen.top/gtxsggicul.html

#endif
来源：http://hz.tian-w.cn/gtxhfkjymr.html

[S31] C++：Hello World
来源：http://hz.zhaomingkeji.xyz/gtcieixxmw.html

#include <iostream>
来源：http://hz.guannengcc.top/gtkcmcqsay.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gttmysiqnf.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gtgrquimcu.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gtmpklfgth.html

[S33] C++：vector 增删
来源：http://hz.yj202588.top/gtkuulwrzq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtipcyakip.html

[S34] C++：遍历 vector
来源：http://hz.xuanzx.com/gtkwqiwxvf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtuklbdwsx.html

[S35] C++：map
来源：http://hz.sysykeji.top/gtfxojipkd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtdfmnxpcj.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gttfiecxch.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtdobcicmg.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gtolsdxlja.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gthgtcayzn.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gtmhafmhsf.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtstfmoxkq.html

[S39] C++：自定义比较器排序
来源：http://hz.feifeiyinyue.top/gtjmznwmkb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuanzhike.top/gtvzonivxm.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtcsqsugih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yueranfly.top/gtrgicralq.html

[S41] C++：类与构造函数
来源：http://hz.dashuyun.cn/gtsxdtzsnk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.havefunace.top/gtygpcjqvh.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtfincovtn.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtfrrcljrp.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gthobkciqg.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gtmxnbivcu.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtschqotun.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtrqcdfguj.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtpokjhcre.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.redwolf501.top/gtfulepimr.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtrqahidhq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtqbwwzhsy.html

[S47] C++：结构化绑定遍历
来源：http://hz.c1oappe.top/gtqhmtyqmp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtmqxpytvt.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtvevttyox.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gttfhjshvn.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtwiauleqk.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtrshwcgdo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigfzy.top/gtrryznbhn.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gtzdbkbjkd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ivvv.top/gtbelrzmgu.html

[S51] C++：显式类型转换
来源：http://hz.guowangkeji.top/gtxcujzctv.html

static_cast<double>(a) / b
来源：http://hz.vqdsnc.cn/gtjymgceug.html

[S52] C++：const 与 noexcept
来源：http://hz.vqdsnc.cn/gtsbjwzdmd.html

int size() const noexcept { return n_; }
来源：http://hz.chenzaomai.com/gtesjjykuh.html

[S53] C++：移动语义
来源：http://hz.daxiang520.top/gtxrygocxo.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtfiqmjeob.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtwyjnndze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.birdmap.top/gtnmcgctdr.html

[S55] C++：结构化绑定
来源：http://hz.jinghuilouyu.cn/gtuuhddelp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtjkokuzxp.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtycflzyta.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtpiakhlmu.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtnpmdwywm.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtmvcfgvhz.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtvpvxqppq.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtembyxlcm.html

[S59] C++：静态断言
来源：http://hz.iojbl.cn/gtdhawxqpu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtupsittlz.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtudybmyik.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhaomingkeji.xyz/gturnxpjqi.html

================================================================================
来源：http://hz.chenlongwang.top/gtasfpxeir.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtgcpgmdla.html

================================================================================
来源：http://hz.yuanzhike.top/gtpdvkmdwb.html

[T01] Kotlin：Hello World
来源：http://hz.jianghu66.top/gtmzvdbyoe.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtkvvsgugt.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtloxwlzfy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.316326.xyz/gtdtliwshd.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtwlszjpsn.html

"值: $b"
来源：http://hz.yonumen.top/gtyxeuqdde.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gtetjxginr.html

val n: String? = null;  n?.length
来源：http://hz.kuanghao11.cn/gtshmqisze.html

[T05] Kotlin：when 表达式
来源：http://hz.svipenyu.cn/gtkgafjgrx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtuzdhrlqh.html

[T06] Kotlin：集合映射
来源：http://hz.shuidangran.top/gtjinenytk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtxmaindng.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtddhxsnkk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.andypj.xyz/gtitozcnlg.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gtntmmuhlu.html

data class User(val name: String, val age: Int)
来源：http://hz.nwbrower.top/gtkjkvlqux.html

[T09] Kotlin：扩展函数
来源：http://hz.chenzaomai.com/gtnwtwepgx.html

fun String.exclaim() = this + "!"
来源：http://hz.mhx1999.top/gtymxwnkmy.html

[T10] Kotlin：默认参数
来源：http://hz.52xcode.cn/gtkxidtrtk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtsbmocmhg.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtlobvosrp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hammf.cn/gtqdngpvhx.html

[T12] Kotlin：解构声明
来源：http://hz.jianghu66.top/gtzshazcix.html

val (a, b) = Pair(1, 2)
来源：http://hz.pengpengdd.cyou/gtaydjjpjd.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtsyfqohwu.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtuthkqlmo.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtbagsntsj.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtotthmvzk.html


<!-- 参考信息 -->