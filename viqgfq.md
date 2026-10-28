代发 wailian999

esac
来源：http://hz.nanxuanxn.top/gtlspcckaz.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtvufiyyut.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pycfn.com/gtchpxzsnf.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtzoxlvotr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.svipenyu.cn/gtfgipsbzs.html

[R14] C 风格 for
来源：http://hz.zhijiandao.cn/gtyfretbzo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gtyfzhbeaa.html

[R15] while 逐行读文件
来源：http://hz.hammf.cn/gtdnbtsuqv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtwrynidaj.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtyxqiijeq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtsilkxeei.html

[R17] 数组定义与取值
来源：http://hz.cashguo.top/gttxizklkn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtvzvtpqql.html

[R18] 遍历数组
来源：http://hz.zhengqikj.top/gtadrukems.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gtetbumpiz.html

[R19] 数组长度
来源：http://hz.hongshengwenyu.top/gthqyzlbgh.html

echo "${#arr[@]}"
来源：http://hz.cheryme.top/gtdwxubgks.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtrabnzjaw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtassnhtfr.html

[R21] 字符串长度
来源：http://hz.gzhubu.top/gthqwtuqbr.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtbqztacpr.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gtrrxtcjzt.html

echo "${s:0:5}"
来源：http://hz.fzhhl.top/gtolqqderw.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtlxobilog.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtvcnyspje.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gtsckvmpdd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gtytqosjxl.html

[R25] 去后缀 / 去前缀
来源：http://hz.aibaodan.cn/gtlzbxhbpx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtpbmtrlwu.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gtgozcslda.html

now=$(date +%F); echo "$now"
来源：http://hz.cashguo.top/gtiwhiypui.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtcmcmascb.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtultzeycn.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtoprrndhr.html

echo "scale=2; 10/3" | bc
来源：http://hz.andypj.xyz/gtltojrwyc.html

[R29] 定义函数
来源：http://hz.wangshuangyany.cn/gtvlwlqocj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtkxgqsxnx.html

[R30] 函数返回状态码
来源：http://hz.yongpay.top/gtjtllsrrj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhiwuduotai.top/gtrzxterun.html

[R31] 局部变量
来源：http://hz.0kj1m.cn/gtymmzefiq.html

f() { local x=1; echo "$x"; }
来源：http://hz.cqqwz.cn/gtidgamxyt.html

[R32] 参数个数校验
来源：http://hz.xziqi.cn/gtnvwtsaab.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.9152youxi.cn/gtmpmhrzyh.html

[R33] 捕获错误并提示行号
来源：http://hz.xylfe.cn/gtqqdmkyuj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtyhaicqbd.html

[R34] 退出时清理
来源：http://hz.sysykeji.top/gtbfqdglru.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtvlncnkly.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gtatokksor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.316326.xyz/gtaxaufojf.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtmdzbcelu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hfpthk.cn/gtbwecjjce.html

[R37] 把输出赋给变量
来源：http://hz.ivvv.top/gtveamsclr.html

files=$(ls -1)
来源：http://hz.zycfv.cn/gtqmjsgyyj.html

[R38] 管道串联
来源：http://hz.tianlin.xyz/gtslxalsll.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtqxwrmvyp.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtudjzpcdk.html

cmd > out.log 2>&1
来源：http://hz.zdqjudy.top/gtqlyqzhtq.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtrjpnrhln.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtfigstekp.html

[R41] 丢弃输出
来源：http://hz.ybcxt.top/gtfssnscyf.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtskqcuehx.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtoxqgrdcx.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtjmbinlnu.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gtnyezrtlo.html

find . -name "*.log" -type f
来源：http://hz.dianchejie.cn/gtbblstvps.html

[R44] 按修改时间查找
来源：http://hz.sysykeji.top/gttmaamymv.html

find . -mtime -7 -type f
来源：http://hz.yj20258.top/gtvzfubcxz.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtutxciyyn.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtszubhnwk.html

[R46] 递归替换文件内容
来源：http://hz.wangdashe.top/gtareyvkdr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtvryguynv.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtuvozjlyl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtaursdwmg.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtfybixuxg.html

awk '{print $1, $3}' a.txt
来源：http://hz.jyoumei.cn/gtdtjhldbb.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gtyzgjxdna.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gtyjqccbzm.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gtcpnwdktl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnxiangtu.top/gtxhoyucin.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtlaxavscs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinghuilouyu.cn/gtvrjjwxaw.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtsbyskvcq.html

wc -l a.txt
来源：http://hz.zdqjudy.top/gtmgxysnxg.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtwkjimshk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtlvcjoeqh.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gtrxpynvmb.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtsmnnvjsp.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtksltpdkr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtsvrbhwys.html

[R56] 远程拷贝
来源：http://hz.wangshuangyany.cn/gtviuhvjtv.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtkxyiijbd.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtqznatgam.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangkeji.top/gtfiyougsa.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gtlrqtsfij.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtgipztkll.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtzkpskyzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtbubogvhv.html

[R60] 只看 HTTP 状态码
来源：http://hz.tianlin.xyz/gtrfdmzmpi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtxprvdkde.html

[R61] 磁盘占用
来源：http://hz.tanke756.top/gtuipzwzqa.html

df -h;  du -sh *
来源：http://hz.vqdsnc.cn/gtkmdvhade.html

[R62] 找最占空间的文件
来源：http://hz.meibo888.top/gtsuitwnlv.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258888.top/gthzuxosjf.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtpwbqjbzd.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtazovnkno.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtczypmnpv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gotoacloud.top/gtqffzqlsz.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtxqovobpn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gtqidgssqc.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gtlcpnecut.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtmubnasvt.html

[R67] 生成随机十六进制串
来源：http://hz.redwolf501.top/gtvzpzkvep.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtsyostwjl.html

[R68] 计算文件校验值
来源：http://hz.cashguo.top/gtbkpcklll.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gtuvkprjql.html

[R69] 生成随机密码
来源：http://hz.hysaishi.cn/gtjqaantax.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtvzlabdqq.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtkexbvtvx.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gtrcakwzhw.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtnyoldeic.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtlvenmphn.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtcvnnaekv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gteijkxauu.html

[R73] 分割大日志
来源：http://hz.jinqigufen.top/gtvlenxjcb.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gthwhgqvld.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtmsbnlzgb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cheryme.top/gthttzrmkq.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtbaavwhwy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gtebkpbdty.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtqcbnqern.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtlbrjrvcp.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtoajsonnt.html

read -rp "请输入: " ans
来源：http://hz.hnxiangtu.top/gtgcjyofqm.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtgqefnlua.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtozsuesdn.html

[R79] 解析命令行选项
来源：http://hz.yuanzhike.top/gtusidibnb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ivvv.top/gtaojtfusx.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtltosztve.html

time ./run.sh
来源：http://hz.zhongyouzk.top/gtscbarfic.html

================================================================================
来源：http://hz.ppjwa.cn/gtznvnswqd.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtztnbosym.html

================================================================================
来源：http://hz.ybcxt.top/gtpelnzzyc.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtblzbakzv.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtgxxyphuc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtgbjhfkhf.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtyzlookpc.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtbmfpbohu.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtegawxcsw.html

int x; scanf("%d", &x);
来源：http://hz.yj20258888.top/gtmkgcswng.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gtcmynuupz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtyfqcdfki.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtwhgkoemh.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtunwfbxga.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtwedtwhip.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gtspudckii.html

[S07] C：数组遍历求和
来源：http://hz.chenlongwang.top/gtjkdyseoi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ehwqpu.com/gtdcywvfzt.html

[S08] C：动态内存分配与释放
来源：http://hz.cqqwz.cn/gtbxraqssu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtrrnsxlkq.html

[S09] C：结构体定义与初始化
来源：http://hz.guowangkeji.top/gtpszfnwhc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtqefbxsjo.html

[S10] C：指针与解引用
来源：http://hz.yuxming.cn/gtzakzxtfh.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtrwbhjdxt.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtfkgzlbbl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gthehebcqq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shangyingyoupin.top/gtqwzawtvx.html

fclose(f);
来源：http://hz.havefunace.top/gtajqnwejc.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtartvnpck.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtixzhlbth.html

[S13] C：宏定义
来源：http://hz.dianchejie.cn/gtfzeadyqr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daria6918.cn/gtnyzyhfwf.html

[S14] C：枚举
来源：http://hz.nwbrower.top/gtpbtfwacg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.svipenyu.cn/gtemgcbvjt.html

[S15] C：类型转换
来源：http://hz.52xcode.cn/gthoopfvxm.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtpnlfcriv.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gttmjjxvos.html

x |= (1 << 3);
来源：http://hz.aizwys.cn/gtqhjqdsat.html

[S17] C：安全拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtzwfivyxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtwawgvick.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtomxjaoms.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtyzskwsig.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gtissqfzrj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtctlfrkiw.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtrnshicfw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtuzwykygz.html

[S21] C：字符类别判断
来源：http://hz.xingfuxueyuan.xyz/gtndwdfrmr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gtruqrbwzv.html

[S22] C：字符串转数字
来源：http://hz.ydjk.org.cn/gtajzkzche.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sweek.top/gtpvacaqzn.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtflegmswa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.mhx1999.top/gthwuqxrqv.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gtuanlrkcb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cheryme.top/gtjmyjudlb.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtmjfbvhxd.html

memcpy(dst, src, n);
来源：http://hz.andypj.xyz/gtbdfivzxr.html

[S26] C：内存清零
来源：http://hz.meibo888.top/gtskvexsci.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gthrupenpm.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gtoakltgaj.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtvbabeuhk.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtseogysfn.html

static int counter = 0;
来源：http://hz.hnxiangtu.top/gtcytpicuo.html

[S29] C：变参函数
来源：http://hz.yongpay.top/gtvmvbsmah.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtywljpgat.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtdxytwsue.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtndunpkzx.html

#define X_H
来源：http://hz.pycfn.com/gtfaqglzvb.html

#endif
来源：http://hz.redwolf501.top/gtgcjspmjk.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtftfpiroz.html

#include <iostream>
来源：http://hz.ydzc1.top/gtaohtwcli.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtoqpbajvq.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtuurfvegh.html

std::string s = "hi";  s += "!";
来源：http://hz.yangfankeji.com/gteapplihb.html

[S33] C++：vector 增删
来源：http://hz.cdnleiting.top/gtrcklpsgv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guowangkeji.top/gtnbqptcfo.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtsmtkgozk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tian-w.cn/gtcrfygjab.html

[S35] C++：map
来源：http://hz.andypj.xyz/gtaszhvpcd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtmmjejayy.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gteydjhwpe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtypgmtdxq.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtppaleips.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.316326.xyz/gtgabdtcnd.html

[S38] C++：排序
来源：http://hz.shangyingyoupin.top/gtqmaahmbt.html

std::sort(v.begin(), v.end());
来源：http://hz.yonumen.top/gtnrlcnzml.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtlxphraey.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtmkeptuxc.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtkeljadwz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtntpffsdq.html

[S41] C++：类与构造函数
来源：http://hz.xylfe.cn/gttkaeyytr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtkbplyhqs.html

[S42] C++：继承与虚函数
来源：http://hz.zdqjudy.top/gtdpumxuku.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtjpovttga.html

[S43] C++：智能指针
来源：http://hz.zhixingplan.top/gtwqdlqcik.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtrmphjqcf.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtqhgzkotz.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtwmvfneeq.html

[S45] C++：lambda
来源：http://hz.guowangkeji.top/gtimernsqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtiskatuxi.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtibhauoxh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gtetucfmgx.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtbepjwdry.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtrqnwgpvd.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gtqhqkdyzw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dianchejie.cn/gtrpotxiol.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtuywhlyyi.html

[S49] C++：写文件
来源：http://hz.zhengqikj.top/gterjhokyl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gttmpgmgxf.html

[S50] C++：格式化数字
来源：http://hz.yvedp.cn/gtrdxrexsg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtpipjthry.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtafvdfwmr.html

static_cast<double>(a) / b
来源：http://hz.zdqjudy.top/gttnufyxai.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gtdpeffwiw.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gteprozqra.html

[S53] C++：移动语义
来源：http://hz.yvedp.cn/gtjqehmaop.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtxdxjikhc.html

[S54] C++：异常处理
来源：http://hz.dianchejie.cn/gtipzlyfqy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtvxhagnan.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtzlytprvk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gtqyipugim.html

[S56] C++：optional
来源：http://hz.haohaochexian.top/gtbsinrshh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gttviszvvt.html

[S57] C++：编译期常量
来源：http://hz.yonumen.top/gtjkzurvnm.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtavsyikva.html

[S58] C++：命名空间
来源：http://hz.tanke756.top/gtzmzkcryp.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gthhakdegn.html

[S59] C++：静态断言
来源：http://hz.kuanghao11.cn/gtejxpplrc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtxdkpqyof.html

[S60] C++：遍历并删除元素
来源：http://hz.gotoacloud.top/gtbgnfbqij.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gtjurxvzij.html

================================================================================
来源：http://hz.xylfe.cn/gthejymanf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtcikaiouc.html

================================================================================
来源：http://hz.sysykeji.top/gtxgxfppgv.html

[T01] Kotlin：Hello World
来源：http://hz.tian-w.cn/gthwdkhoxg.html

println("Hello")
来源：http://hz.snrcjt.cn/gtrufuvioy.html

[T02] Kotlin：变量
来源：http://hz.meibo888.top/gtwkaqntfe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.redwolf501.top/gtgfrrvsao.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gtzzmvyrvb.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtmdisrogo.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtgobmearz.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtweoodxot.html

[T05] Kotlin：when 表达式
来源：http://hz.svipenyu.cn/gtlmdmhepr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtxbjagojj.html

[T06] Kotlin：集合映射
来源：http://hz.zhengqikj.top/gtojhdlxdq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtqtjxhcmy.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxinkj.top/gthwfwvblc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aizwys.cn/gtgjrociaj.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtjkuwduxz.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtywgwxpli.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtbjcjpzhc.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigfzy.top/gthbcvlfys.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtdaftzfqv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cashguo.top/gtzfzahhsa.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangkeji.top/gtyweaomio.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.iojbl.cn/gtxvqbuwys.html

[T12] Kotlin：解构声明
来源：http://hz.chenzaomai.com/gtzbegexeb.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtlmudvfxi.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtxhbveint.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtahknffmb.html

[T14] Kotlin：循环
来源：http://hz.hammf.cn/gtvbzqylkw.html

for (i in 1..10) println(i)
来源：http://hz.yangfankeji.com/gttimnznzu.html


<!-- 参考信息 -->