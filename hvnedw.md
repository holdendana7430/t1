代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtndozcxou.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtuuighthk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gttvqwrvnf.html

[R15] while 逐行读文件
来源：http://hz.zhengqikj.top/gtitmwrbns.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gtecrlcdyp.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gtvtawarbv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gtyfvedifw.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtpujyznjz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtxcepyjks.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gtqlgkvjnf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ywan-chungtsiang.top/gtiyrjdchu.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gtorrhyrtl.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtufshvkro.html

[R20] 关联数组（字典）
来源：http://hz.0kj1m.cn/gtrjvvyykc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnqzz.top/gtfpctzufx.html

[R21] 字符串长度
来源：http://hz.aibaodan.cn/gtsqwiprwd.html

echo "${#s}"
来源：http://hz.birdmap.top/gtisgkaust.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtigaaeqzx.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtjqymkslh.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtvpxaxehw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hammf.cn/gtczqmadwk.html

[R24] 大小写转换
来源：http://hz.jiagoushi.top/gtwjvietwj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtidpwnedz.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtxqxopfmw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.316326.xyz/gtuwilvopm.html

[R26] 命令替换
来源：http://hz.gogol.net.cn/gtjgepouka.html

now=$(date +%F); echo "$now"
来源：http://hz.chenlongwang.top/gtmdgbeims.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gttmhfwcgz.html

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtbugyawje.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtpvyfgzgn.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtvxqxstih.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gteehjpsio.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgufenzy.top/gtcuhccjud.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtntlrrdes.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtrmwzjpfb.html

[R31] 局部变量
来源：http://hz.cheryme.top/gtmtcoqvxg.html

f() { local x=1; echo "$x"; }
来源：http://hz.hysaishi.cn/gtgwmpsich.html

[R32] 参数个数校验
来源：http://hz.guowangkeji.top/gtrxvkoenx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.haohaochexian.top/gtpxfbqenz.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtlucfxhib.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gttzfctjts.html

[R34] 退出时清理
来源：http://hz.chenzaomai.com/gtosndrtpe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtsxitdshx.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtyexbnawb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gtomvurtrf.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtwwxoeunj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gteneivmmr.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gtmlrdpxis.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtxieqpbpe.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtlzgehsqv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtvhyocdgk.html

[R39] 重定向标准输出与错误
来源：http://hz.haohaochexian.top/gtcqwmqipj.html

cmd > out.log 2>&1
来源：http://hz.aibaodan.cn/gtnqfxmned.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gtcrkdslld.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtrgkhfsmd.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtigyrufxm.html

cmd >/dev/null 2>&1
来源：http://hz.jqgfzy.top/gtcbfyxicw.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtnwmnvulx.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtunzzstqs.html

[R43] 按名字查找文件
来源：http://hz.haohaochexian.top/gtrcuwdzkp.html

find . -name "*.log" -type f
来源：http://hz.xylfe.cn/gtkctpverl.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtucbsdidh.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtrsqztcsw.html

[R45] 批量删除
来源：http://hz.bjfxy.top/gteqyuitmq.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtluvtyvck.html

[R46] 递归替换文件内容
来源：http://hz.sysykeji.top/gthxkpgqns.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gthaiiorbn.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtppcmhpua.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gtqifxzkcs.html

[R48] awk 取指定列
来源：http://hz.hongshengwenyu.top/gtoumfkiro.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtibgigzbu.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtyopnjrnx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtmelgsuwu.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtbdbhakui.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258.top/gtdodhskbo.html

[R51] 排序去重取前几
来源：http://hz.svipenyu.cn/gtvbuosfep.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtpkzicvyk.html

[R52] 统计行数
来源：http://hz.jinghuilouyu.cn/gttlbfkzzn.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtwrcwzwkn.html

[R53] 查看文件头与实时尾
来源：http://hz.cashguo.top/gtenogarvz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtknnnsohq.html

[R54] 比较两个文件
来源：http://hz.pycfn.com/gtsqzbkfnp.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtmfmfwbfn.html

[R55] 压缩与解压
来源：http://hz.mhx1999.top/gtysurrcjy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.haohaochexian.top/gtxvztboby.html

[R56] 远程拷贝
来源：http://hz.xylfe.cn/gtlhuhoigw.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gteyvoegpl.html

[R57] 远程执行命令
来源：http://hz.pengpengdd.cyou/gtmmullzpe.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtqkgoseuh.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtrodmvhxp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gtjjkgihml.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtpzhkmasp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.haohaochexian.top/gtqwpllffg.html

[R60] 只看 HTTP 状态码
来源：http://hz.yueranfly.top/gtxertofpd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sufxvd.cn/gtacqzgire.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtrjyzdjme.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtaawcgton.html

[R62] 找最占空间的文件
来源：http://hz.ydjk.org.cn/gtjhxmxmpa.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtvveoeaaj.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtbybjfnzh.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtpfqpuaqf.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtpkbwmxnb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtgbfucpje.html

[R65] 查看端口占用
来源：http://hz.ydzc1.top/gtpmwnailr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhaomingkeji.xyz/gtdzbvlprq.html

[R66] 定时任务
来源：http://hz.cqqwz.cn/gtrumnnuxa.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gtteelsjxg.html

[R67] 生成随机十六进制串
来源：http://hz.zhiwuduotai.top/gtcbenhxzy.html

openssl rand -hex 16
来源：http://hz.vqdsnc.cn/gtgdmyzyka.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtccvnqwyi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtmckdpyis.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtnbvamgbx.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtmxcizxac.html

[R70] 时间戳与互转
来源：http://hz.fzhhl.top/gtrsnxwkef.html

date +%s;  date -d @1700000000
来源：http://hz.gaohongyu789.top/gtnbefdpnq.html

[R71] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtofkvxlup.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtkylunuur.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtzzitdaih.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gtpmpaiytc.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtexuyzuui.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtuuyymtrv.html

[R74] 批量重命名
来源：http://hz.daria6918.cn/gtopvehquf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtqectbvti.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtyusoblts.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtosfjxasp.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtjnnhgiik.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gttfavqsqf.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gtnrprggce.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtcexwmctj.html

[R78] 交互式菜单
来源：http://hz.zdqjudy.top/gtsqybemnn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yonumen.top/gtyujbvgui.html

[R79] 解析命令行选项
来源：http://hz.svipenyu.cn/gtmthwttqi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtqxghtvwv.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtsgjofsli.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtdphghime.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtnrpqsfyp.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtlwcmvvbc.html

================================================================================
来源：http://hz.0kj1m.cn/gtpgojzaoq.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtyznnrzen.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtxhuzbgmu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhaomingkeji.xyz/gtueofchva.html

[S02] C：变量与格式化输出
来源：http://hz.xziqi.cn/gttqaueyzo.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinghuilouyu.cn/gtkomsmoyw.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtkbealekq.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtgnhzlcnd.html

[S04] C：字符串复制
来源：http://hz.jqgfzy.top/gtbvthaiwx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gogol.net.cn/gtrydtuafj.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtpyfnwucq.html

strlen(s)
来源：http://hz.shuidangran.top/gtoauqatqi.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtrxyhapmp.html

strcmp(a, b) == 0
来源：http://hz.snrcjt.cn/gtjbrgcjnt.html

[S07] C：数组遍历求和
来源：http://hz.gzhubu.top/gtrptkbahh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtfntycovs.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtbpiwfojq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cqqwz.cn/gtppssdrpz.html

[S09] C：结构体定义与初始化
来源：http://hz.shzxlz.cn/gtiwoqyrax.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.haohaochexian.top/gtajbwqgcb.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gteqqweohy.html

int *p = &a;  *p = 5;
来源：http://hz.gzhubu.top/gtphirnvrw.html

[S11] C：逐行读文件
来源：http://hz.tanke756.top/gtspyhlijb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtoeautbmw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gtzdvvenaa.html

fclose(f);
来源：http://hz.hnqzz.top/gtejtgpdhg.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gtygeeukdf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtiilcistj.html

[S13] C：宏定义
来源：http://hz.chenzaomai.com/gtinsctokk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.quarkkingdee.top/gtwgpqgtci.html

[S14] C：枚举
来源：http://hz.snrcjt.cn/gtfdfespag.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aibaodan.cn/gthecofnix.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gttmdfwezp.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtlithbahs.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtfihnfdxq.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtfvpjbnyu.html

[S17] C：安全拼接字符串
来源：http://hz.zhijiandao.cn/gtfkygzwvd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nwbrower.top/gtsfpndzbl.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtlccqiyza.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtbvjnucxf.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtnxbsqujl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtvxvyhyau.html

[S20] C：二分查找
来源：http://hz.vqdsnc.cn/gtckwjfmlk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtjpolewbi.html

[S21] C：字符类别判断
来源：http://hz.guannengcc.top/gtrtcsvcxi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.svipenyu.cn/gtmprlipfh.html

[S22] C：字符串转数字
来源：http://hz.vqdsnc.cn/gtgxsclcjy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gtvrgoatxz.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtphbzpzjd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.aizwys.cn/gtgbyitamm.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtjywbvskv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtjowauhbk.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtmgxsuwpy.html

memcpy(dst, src, n);
来源：http://hz.shuidangran.top/gttnrrqwtm.html

[S26] C：内存清零
来源：http://hz.yuxming.cn/gtmckkwdta.html

memset(a, 0, sizeof a);
来源：http://hz.yvedp.cn/gtzgjictjd.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gtsyhmbksk.html

const double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtisnocwvd.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtuvikfnac.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtwwbzacte.html

[S29] C：变参函数
来源：http://hz.yuxming.cn/gtxtqjruow.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.316326.xyz/gtxtnaphec.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtpilmibnz.html

#ifndef X_H
来源：http://hz.cheryme.top/gtgwxaasad.html

#define X_H
来源：http://hz.tanke756.top/gtnwohxglr.html

#endif
来源：http://hz.yongpay.top/gtofkzsxwk.html

[S31] C++：Hello World
来源：http://hz.hongshengwenyu.top/gtlabyfhui.html

#include <iostream>
来源：http://hz.mhx1999.top/gtdfsxjqqt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.smart0.xyz/gtiggsarav.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gtwiopceuu.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtcejlmydj.html

[S33] C++：vector 增删
来源：http://hz.chenjidiqi.icu/gtazwmweze.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gtgfknxtwh.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtjelxtgea.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtfyxaipuv.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtesjwjbui.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtabrozhvp.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtoggifzrq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gthmgwdfnx.html

[S37] C++：set
来源：http://hz.meibo888.top/gtrahywyag.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtgxhdkttk.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtdzjgqhyr.html

std::sort(v.begin(), v.end());
来源：http://hz.yonumen.top/gtemqrjhgg.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtyilvaqvf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtqzbxqigm.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtgrmnotkm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtkkogjjey.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtuzqrylpx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigufen.top/gtsuzzakww.html

[S42] C++：继承与虚函数
来源：http://hz.aizwys.cn/gttyzvmogi.html

class B : public Base { public: void f() override {} };
来源：http://hz.jianghu66.top/gttknutabg.html

[S43] C++：智能指针
来源：http://hz.jinghuilouyu.cn/gtnwczuelb.html

auto p = std::make_unique<int>(5);
来源：http://hz.c1oappe.top/gtbmglodgl.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtxsctbsfb.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gtignugchr.html

[S45] C++：lambda
来源：http://hz.hnqzz.top/gtchmgwiqh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtuqqfevqg.html

[S46] C++：函数模板
来源：http://hz.vqdsnc.cn/gtoiekyjyt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sweek.top/gtjgmvxadl.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhengqikj.top/gtyayolkft.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtfvbzfkjc.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtsmypdxap.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gtqbbwsodi.html

while (std::getline(in, line)) { }
来源：http://hz.52xcode.cn/gtipnnxigy.html

[S49] C++：写文件
来源：http://hz.quarkkingdee.top/gtexglwstv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shangyingyoupin.top/gtwpteesib.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtmxaspmyo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gtollbazge.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtxywnjcbn.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtapxzjpln.html

[S52] C++：const 与 noexcept
来源：http://hz.birdmap.top/gtoonsaczo.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtbnynorou.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtfcmslxey.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtaewxtyoi.html

[S54] C++：异常处理
来源：http://hz.fengsongda.top/gtyncpcfob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shuidangran.top/gtouzcqhak.html

[S55] C++：结构化绑定
来源：http://hz.sxryk.cn/gtpeagixzq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtrwrwkvjm.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtmdlfnmhl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtumlzsvjb.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtztwuvlxd.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtnbhadylw.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtyqadtvdz.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhixingplan.top/gtdaysjfch.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtupmwkpfu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aizwys.cn/gtcggyaymo.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtzrmjfopb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtfeybiqaf.html

================================================================================
来源：http://hz.snrcjt.cn/gtfspkcweu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtzntugrnx.html

================================================================================
来源：http://hz.jiagoushi.top/gtobdlbvor.html

[T01] Kotlin：Hello World
来源：http://hz.ywan-chungtsiang.top/gtdmwhuivv.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtfvwkruhu.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtmmqhhslj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ywan-chungtsiang.top/gtnetlrnrw.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gtlygtufqp.html

"值: $b"
来源：http://hz.zdqjudy.top/gtccxdukph.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtgthrdbpj.html

val n: String? = null;  n?.length
来源：http://hz.nanxinkj.top/gtfjfzbvre.html

[T05] Kotlin：when 表达式
来源：http://hz.hfpthk.cn/gtavepqaqi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgufenzy.top/gtbvnjjiet.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtucrpfwdc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yueranfly.top/gtcsznwodq.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtccamgxvh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtctvbhywo.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtupqwroln.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxinkj.top/gtzkzlsfha.html

[T09] Kotlin：扩展函数
来源：http://hz.jinyuanbaomall.cn/gtmmcrfrtd.html

fun String.exclaim() = this + "!"
来源：http://hz.yj202588.top/gtrxprrvdm.html

[T10] Kotlin：默认参数
来源：http://hz.gaohongyu789.top/gtjfyqgbvk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xinyue.icu/gtukpfglys.html

[T11] Kotlin：协程
来源：http://hz.jinqigufen.top/gtyxxfqppc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuanzhike.top/gtqovrdrfs.html

[T12] Kotlin：解构声明
来源：http://hz.jianghu66.top/gttpueukzn.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtlqhcklzc.html

[T13] Kotlin：只读 Map
来源：http://hz.zdqjudy.top/gteerrohif.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtnbeenrbf.html

[T14] Kotlin：循环
来源：http://hz.andypj.xyz/gtyhrgpwzc.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gthgeotddc.html

[T15] Kotlin：接口
来源：http://hz.0kj1m.cn/gtifderxyk.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtmxgajhbn.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangtech.top/gtnkvaswbi.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtrwfspnkg.html


<!-- 参考信息 -->