代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tian-w.cn/gtrvcajnur.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtpvbjvkmu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gttzjsplki.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtymyarsof.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtpxrpixur.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gthixjegpj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gttjamekmu.html

[R19] 数组长度
来源：http://hz.sweek.top/gtzpymxgaf.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtnogycxhi.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gthyndwfhi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhiwuduotai.top/gtspunewzk.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gtutdrmecp.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtmybkwsxs.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtejdavovb.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtmkaxwwdg.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gttmrhzmde.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtwjewiqub.html

[R24] 大小写转换
来源：http://hz.andypj.xyz/gtqolroxzk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gtkqyqwyge.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtlxiaitxr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtshmdnhmm.html

[R26] 命令替换
来源：http://hz.havefunace.top/gthmvjgidv.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gthjdyzmpp.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtvqvglqhe.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtgfpbgssn.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtqizqenrx.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gtvcvousea.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtcwuhfuml.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dashuyun.cn/gtpeouxdum.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gtlmlxdypl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtcdktnawx.html

[R31] 局部变量
来源：http://hz.zhoulong.xyz/gtoioypyiq.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtofayxfdp.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtrucoowlb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtfoubtzvl.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgfzy.top/gtbgukmtjp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtlourddaz.html

[R34] 退出时清理
来源：http://hz.svipenyu.cn/gtoayfjbew.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtonagpcst.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtylzlyjhm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhoulong.xyz/gtczzobwax.html

[R36] 并发执行多个任务
来源：http://hz.c1oappe.top/gthiiijwnw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gtgyprxcse.html

[R37] 把输出赋给变量
来源：http://hz.gaohongyu789.top/gtuymskjtu.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtozqfahzw.html

[R38] 管道串联
来源：http://hz.zhiwuduotai.top/gtemaqppsc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cheryme.top/gtkjqoiybb.html

[R39] 重定向标准输出与错误
来源：http://hz.fzhhl.top/gtxecumldi.html

cmd > out.log 2>&1
来源：http://hz.dianchejie.cn/gtpqaopzhl.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtudrdlwvu.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtuybibhdh.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtolzoqera.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangtech.top/gtgdjzzkfj.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtohzwnzvo.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtjdzhjckn.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtvzfrxzbj.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gtwwgdhocu.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtcylopfhr.html

find . -mtime -7 -type f
来源：http://hz.sufxvd.cn/gtyouuusik.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtjrdwgqie.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtddnmckws.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtujsftsvd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhengqikj.top/gtvansakyk.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtjhwmmuel.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtbwrlbwsv.html

[R48] awk 取指定列
来源：http://hz.gaohongyu789.top/gtdlnvgtbc.html

awk '{print $1, $3}' a.txt
来源：http://hz.vqdsnc.cn/gtjezxgkpu.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtlwfcyywv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtckuptwaj.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtreddtwid.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigfzy.top/gtuggkjbst.html

[R51] 排序去重取前几
来源：http://hz.yvedp.cn/gttkypeppr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtgrhogfap.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtdcvzaifb.html

wc -l a.txt
来源：http://hz.sufxvd.cn/gtbifjzvaz.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtppvfjwsg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtztulgexw.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtxeyvzbui.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtukyyniel.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtitydhmyv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtmzqhucho.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtsgrpyghn.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtoakrezdu.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gtjlhnlqab.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gtfyyajwwg.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtmibysgfj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtnlchqjpb.html

[R59] 发 POST JSON
来源：http://hz.feifeiyinyue.top/gtmvhsgzme.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gtjyxnaduw.html

[R60] 只看 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtmozvxsef.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtkgduqeex.html

[R61] 磁盘占用
来源：http://hz.jqgfzy.top/gtcanxqyei.html

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gtticrzlqb.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtrmekivsd.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtzdtxytep.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtweioyxbo.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gticclrxmv.html

[R64] 结束进程
来源：http://hz.shuidangran.top/gtsqjrkxky.html

kill -9 $(pgrep -f app.py)
来源：http://hz.havefunace.top/gtnajkhqvh.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtlpowlqel.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtrnegazbk.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtiskhpdwf.html

crontab -e;  crontab -l
来源：http://hz.vqdsnc.cn/gtleyrrarr.html

[R67] 生成随机十六进制串
来源：http://hz.jqgfzy.top/gthklaqugs.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtrrylxvmz.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtomaaulrn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhijiandao.cn/gttupxessi.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtdhvwjccx.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtqxcpkfoy.html

[R70] 时间戳与互转
来源：http://hz.andypj.xyz/gtwonquzad.html

date +%s;  date -d @1700000000
来源：http://hz.tanke756.top/gtydxcvzuc.html

[R71] 日期格式化
来源：http://hz.sufxvd.cn/gtoqloqeva.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtqsminjaj.html

[R72] 等待端口就绪
来源：http://hz.meibo888.top/gtydtizymi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtttpohqpl.html

[R73] 分割大日志
来源：http://hz.jinqigufen.top/gtibzvwakc.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gtszfoscfb.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtitvdhqtj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jianghu66.top/gtczvnzyso.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtlisqvrlx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.bjfxy.top/gtczcefyld.html

[R76] 使用临时文件
来源：http://hz.jinghuilouyu.cn/gtlhxcqxlx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtgyhqzzkw.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gthmumblsv.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtwmctulpx.html

[R78] 交互式菜单
来源：http://hz.hywenlv.cn/gtxzndhpoz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jlsjyb.cn/gtggcdszco.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtznvejhwo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtmswlrlij.html

[R80] 查看脚本执行耗时
来源：http://hz.ywan-chungtsiang.top/gtriofxqjy.html

time ./run.sh
来源：http://hz.iojbl.cn/gttqutmkvh.html

================================================================================
来源：http://hz.guowangkeji.top/gtbqkfkeyi.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtdypnmhgc.html

================================================================================
来源：http://hz.yj202588.top/gtgnorkjao.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gtvwkwmbkx.html

#include <stdio.h>
来源：http://hz.ybcxt.top/gttbebuzhn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gtvnwedwex.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gttwhgufks.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtpondirqp.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtdchynflf.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtljxzskij.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtccewsryw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gotoacloud.top/gtuqisgfrg.html

[S05] C：字符串长度
来源：http://hz.cashguo.top/gtrlkcckzb.html

strlen(s)
来源：http://hz.hnxiangtu.top/gtpwxgkptf.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtokqjzlhq.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gthuipvubs.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtdtdxfrrq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gtvexoztez.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtwprgqabv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtqjviaypl.html

[S09] C：结构体定义与初始化
来源：http://hz.gogol.net.cn/gtxpnqgmzt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtehjicqtz.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtxrjgqqfi.html

int *p = &a;  *p = 5;
来源：http://hz.vqdsnc.cn/gtwsbxmiba.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtvdejuvpo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtjtrbqtwe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtpiiqfnbv.html

fclose(f);
来源：http://hz.jinqigufen.top/gtfxqjofdb.html

[S12] C：写文件
来源：http://hz.nwbrower.top/gtfixchssy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtsidgiojc.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtnbadnwsa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtmgpuoxcb.html

[S14] C：枚举
来源：http://hz.yueranfly.top/gtmphyhymc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtgjdghzvw.html

[S15] C：类型转换
来源：http://hz.hongshengwenyu.top/gtypuciwtf.html

(double) a / b
来源：http://hz.jiagoushi.top/gtfvweqtre.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gtzdyueykv.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gtemndshhh.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtewwnogss.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtopzfphnf.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtvicqukcr.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gthrhxqlga.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gtcwcrennj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtaderaihg.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtomibqzdk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtvnjctbpz.html

[S21] C：字符类别判断
来源：http://hz.ehwqpu.com/gtfwtcqgqu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nwbrower.top/gtipdncwmp.html

[S22] C：字符串转数字
来源：http://hz.pycfn.com/gtbzwoprha.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tianlin.xyz/gtgulfxmrl.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtvgshskro.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtvgattvuk.html

[S24] C：获取本地时间
来源：http://hz.ydjk.org.cn/gtxfzliwdr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.smart0.xyz/gtznvuwpiw.html

[S25] C：内存拷贝
来源：http://hz.zhijiandao.cn/gtlrzoleth.html

memcpy(dst, src, n);
来源：http://hz.yuxming.cn/gtfgpvjxdd.html

[S26] C：内存清零
来源：http://hz.hnxiangtu.top/gtltwykwhh.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtddbsqbgc.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtnrvmkncj.html

const double PI = 3.14159;
来源：http://hz.nwbrower.top/gtxbrawcpv.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtlheojlgc.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gteavzeqle.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtjoiiheei.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.havefunace.top/gtumilfmip.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtwyaomtia.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtndpehzvf.html

#define X_H
来源：http://hz.sufxvd.cn/gtdkktdtge.html

#endif
来源：http://hz.zhixingplan.top/gtszmabzst.html

[S31] C++：Hello World
来源：http://hz.yuxming.cn/gtrlvqupsd.html

#include <iostream>
来源：http://hz.yueranfly.top/gtrvukuyhp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtylbpqunq.html

[S32] C++：字符串
来源：http://hz.haohaochexian.top/gtzurfcrcx.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtfzrgxydv.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtexbwkogn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtmtwnnazt.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtwiqqwmwz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtisgzccqv.html

[S35] C++：map
来源：http://hz.bjfxy.top/gtqgdijlap.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtatjmslab.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gthvnlqavx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtjqmguqjo.html

[S37] C++：set
来源：http://hz.yj20258888.top/gtzpcgmgfx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.bjfxy.top/gteketngci.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gtqbcsvtjh.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtecfiflqu.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtjlofisju.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtlctdjixh.html

[S40] C++：查找元素
来源：http://hz.meibo888.top/gtmyfbumdn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtpmoohbmh.html

[S41] C++：类与构造函数
来源：http://hz.tanke756.top/gtqkrgsgqf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cdnleiting.top/gtamrmjavy.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gttwehwmza.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gtihcybgpr.html

[S43] C++：智能指针
来源：http://hz.daria6918.cn/gtcgqvfzeh.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhongyouzk.top/gtjmpywobn.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtjcepcsjl.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtphbnxefb.html

[S45] C++：lambda
来源：http://hz.yonumen.top/gtubwdxege.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gteqrooybz.html

[S46] C++：函数模板
来源：http://hz.jiagoushi.top/gtlrteeypz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gtmrtnpqjz.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtvjxcslci.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtqkkdiatr.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtsjmarwhg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtqplrzldv.html

while (std::getline(in, line)) { }
来源：http://hz.svipenyu.cn/gtummhwbpq.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtmimcoase.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258888.top/gtwhnzuolg.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtafvqjxil.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.quarkkingdee.top/gtptdtllws.html

[S51] C++：显式类型转换
来源：http://hz.gaohongyu789.top/gtzvgnqbjf.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gtlpvqhmls.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtfhhqursv.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtomhaxlna.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtthltsyum.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtaroplopv.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtjcnvjwgt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtjlptnusk.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtfunrfyum.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtdakvsafi.html

[S56] C++：optional
来源：http://hz.shuidangran.top/gttchnuvum.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.smart0.xyz/gtnjqidrxg.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtqwltxtjf.html

constexpr int N = 10;
来源：http://hz.hnxiangtu.top/gtiluutevs.html

[S58] C++：命名空间
来源：http://hz.bjfxy.top/gtrqovorjp.html

namespace ns { int f() { return 1; } }
来源：http://hz.jianghu66.top/gtzfannefb.html

[S59] C++：静态断言
来源：http://hz.havefunace.top/gtxqbcyhic.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigfzy.top/gtfbontjxb.html

[S60] C++：遍历并删除元素
来源：http://hz.zhijiandao.cn/gtlqicroqw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtzvohsuqh.html

================================================================================
来源：http://hz.xziqi.cn/gtzjuklozx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nwbrower.top/gtwadiexsg.html

================================================================================
来源：http://hz.gotoacloud.top/gtlzhgqedm.html

[T01] Kotlin：Hello World
来源：http://hz.c1oappe.top/gtnlazwhzt.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtiicmgdyg.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtuhqucpji.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtibsmdtbs.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gthjbnjfbk.html

"值: $b"
来源：http://hz.hnxiangtu.top/gtjtbomrkz.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtdxqbkxxz.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtlqwqisfr.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gttgtzfstz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dashuyun.cn/gtflqkmffw.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtgkugbxoo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtoqlswaww.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgufenzy.top/gtbryajdzn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtwnmnrzdv.html

[T08] Kotlin：数据类
来源：http://hz.wangdashe.top/gtsiyansfn.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtxqdaumcb.html

[T09] Kotlin：扩展函数
来源：http://hz.tanke756.top/gtczvwsfsv.html

fun String.exclaim() = this + "!"
来源：http://hz.tianlin.xyz/gtqcxacgwy.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtrbrhbqnm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtpdimykgi.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtzfmhayyp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hongshengwenyu.top/gthqvvwonn.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtpmkcxtyu.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gttlthqkjb.html

[T13] Kotlin：只读 Map
来源：http://hz.xinyue.icu/gtwskzfdhe.html

val m = mapOf("a" to 1)
来源：http://hz.yuanzhike.top/gtnrajrxwd.html

[T14] Kotlin：循环
来源：http://hz.fzhhl.top/gtudqytohv.html

for (i in 1..10) println(i)
来源：http://hz.yueranfly.top/gtztsrrbgp.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gthjnacfdb.html

interface Shape { fun area(): Double }
来源：http://hz.jlsjyb.cn/gtibongvue.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtcunzzxat.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gttekxehup.html

[T17] Swift：变量与常量
来源：http://hz.snrcjt.cn/gtxwbpwglq.html

var a = 1;  let b = 2
来源：http://hz.shangyingyoupin.top/gttofbcrif.html

[T18] Swift：字符串插值
来源：http://hz.wangshuangyany.cn/gtunrwhwiy.html

"值: \(b)"
来源：http://hz.meibo888.top/gtrvksulxn.html


<!-- 参考信息 -->