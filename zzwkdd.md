代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gtakawutsj.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gttuvbjjzp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtsmdaydlf.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtyazrqieo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.haohaochexian.top/gtbiliipzc.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gteeptlcmb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gtbkdadjzu.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gtfzdjzfbf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ywan-chungtsiang.top/gtimuunoqj.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gthyorgstz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtoxqpmtoc.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtbizzfoua.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gttdqmedci.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gtfmvkvnpm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daria6918.cn/gtfburkuue.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gthuhouvtb.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gthkietfuy.html

[R22] 截取子串
来源：http://hz.tanke756.top/gtknxygwzg.html

echo "${s:0:5}"
来源：http://hz.yanxiufei.cn/gtqedjwhcj.html

[R23] 字符串替换
来源：http://hz.shangyingyoupin.top/gtilksdhfe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cdnleiting.top/gtyjrnixqt.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtombjksue.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ivvv.top/gtngceobvl.html

[R25] 去后缀 / 去前缀
来源：http://hz.svipenyu.cn/gtkflhlbbc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtvwuegdgh.html

[R26] 命令替换
来源：http://hz.shanyushiyangkeji.top/gtjdckwiit.html

now=$(date +%F); echo "$now"
来源：http://hz.hnqzz.top/gtpwchrcxw.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtspgkfmtk.html

echo $((1 + 2 * 3))
来源：http://hz.hongshengwenyu.top/gtjbpwmkvj.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtbfmcddad.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtmdyqqjwr.html

[R29] 定义函数
来源：http://hz.tianlin.xyz/gtzbkleiuy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gtmevfzegv.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangtech.top/gthbmagvkb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yanxiufei.cn/gtiiuwvcsp.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gtfgxohpoc.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtzdurgpas.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtwlfofijj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtjnhqddvp.html

[R33] 捕获错误并提示行号
来源：http://hz.zhaomingkeji.xyz/gtphtdmtvf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jlsjyb.cn/gtyhrastmp.html

[R34] 退出时清理
来源：http://hz.hnxiangtu.top/gtkxvpotvy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtguotrkur.html

[R35] 后台执行并等待
来源：http://hz.52xcode.cn/gtyoslhokq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.316326.xyz/gtglzgdvbb.html

[R36] 并发执行多个任务
来源：http://hz.guannengcc.top/gtxxnohdiz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hywenlv.cn/gtwqsgxila.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gthfjmlgob.html

files=$(ls -1)
来源：http://hz.nanxinkj.top/gtcejjiplu.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtykbxtlzl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtvffrrgjx.html

[R39] 重定向标准输出与错误
来源：http://hz.haohaochexian.top/gtcmsoktwt.html

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtfxfhumcr.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gttpamywgt.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtwndywieq.html

[R41] 丢弃输出
来源：http://hz.jqgufenzy.top/gtbzftkusp.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtmnpmoggw.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gthwldspsa.html

wc -l < a.txt
来源：http://hz.xylfe.cn/gtugbuqxni.html

[R43] 按名字查找文件
来源：http://hz.cheryme.top/gtcrsaeuqu.html

find . -name "*.log" -type f
来源：http://hz.ydjk.org.cn/gtwapxydig.html

[R44] 按修改时间查找
来源：http://hz.andypj.xyz/gtijjkgmcj.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtjhzlbqye.html

[R45] 批量删除
来源：http://hz.chenjidiqi.icu/gtgoyxicpu.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtcljdqktu.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtfpcyxrcn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtqslimppo.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtihdqhqvq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gtqeyoojba.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gtgdbskshd.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gtttyhyzej.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gtzdxvyykz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tian-w.cn/gtwigmlsdm.html

[R50] awk 求和
来源：http://hz.hnxiangtu.top/gtbvfaaqqk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinghuilouyu.cn/gtzqhkpagg.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gtoaoyzuli.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gttgzeqryi.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtoyzpuhlb.html

wc -l a.txt
来源：http://hz.yj202588.top/gtxuvvreab.html

[R53] 查看文件头与实时尾
来源：http://hz.xylfe.cn/gteckcsqxr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtulksszyl.html

[R54] 比较两个文件
来源：http://hz.birdmap.top/gtrgmdncyb.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtzhwfsgnf.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtqxapqsop.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtuzdaiivu.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gtcmgsblok.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gttrchemsh.html

[R57] 远程执行命令
来源：http://hz.cucudq.cn/gtriqnrwfd.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtvbzihefd.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtjyqaxiyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtswuvdhdz.html

[R59] 发 POST JSON
来源：http://hz.vqdsnc.cn/gtscdzcdzp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxinkj.top/gtzqdbcdgr.html

[R60] 只看 HTTP 状态码
来源：http://hz.ivvv.top/gturtomqfy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gteuncgmxz.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtcvlfvico.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gtbqkcwqml.html

[R62] 找最占空间的文件
来源：http://hz.jqgfzy.top/gtwwfzawuc.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtebzlvxxx.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gttcewgjzb.html

free -h;  ps aux | grep nginx
来源：http://hz.sufxvd.cn/gtuzfgbvrx.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtqiywdymi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtpsznhrhd.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtcybmkbwq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtoksxsvnt.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtwtzzirwj.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gthhkruhlc.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gteuqvpodl.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtdcetfxck.html

[R68] 计算文件校验值
来源：http://hz.redwolf501.top/gtkahjpjye.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gogol.net.cn/gtkgcsmqas.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gthkctaqug.html

head -c 16 /dev/urandom | base64
来源：http://hz.gzhubu.top/gtyumahfel.html

[R70] 时间戳与互转
来源：http://hz.yvedp.cn/gtczdikzdd.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtjcftpfwa.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gtudduvidd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fzhhl.top/gtodpucphi.html

[R72] 等待端口就绪
来源：http://hz.havefunace.top/gtstzoiwur.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtzpvbgbcg.html

[R73] 分割大日志
来源：http://hz.ivvv.top/gtzrthstsv.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gthnejmgdw.html

[R74] 批量重命名
来源：http://hz.gzhubu.top/gtffkugxyu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtefhmbgfi.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtifqxpnqx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gttnqmzvnj.html

[R76] 使用临时文件
来源：http://hz.quarkkingdee.top/gtbtjwbfrf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtuzkavelg.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gttrlqqlph.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtvuergxcd.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtaqazvkux.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtcekidxas.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gthaaiawtr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtgqcrczrm.html

[R80] 查看脚本执行耗时
来源：http://hz.ppjwa.cn/gtyuvtaqnk.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtzkiclgom.html

================================================================================
来源：http://hz.vqdsnc.cn/gtacrtjyrw.html

S. C / C++ 专题
来源：http://hz.jinqigfzy.top/gtkdcpnesp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtlymqffna.html

[S01] C：Hello World
来源：http://hz.wangdashe.top/gtfzpufoqi.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtfsjgtfuj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhengqikj.top/gtpenorjoc.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtavipakzf.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtyyyyacth.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gtwdmptxwu.html

int x; scanf("%d", &x);
来源：http://hz.yueranfly.top/gtiuccmtiu.html

[S04] C：字符串复制
来源：http://hz.vqdsnc.cn/gthgrdjhdw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtuurlilmw.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gtlsbhogkm.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gthypljxsj.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtuihgaaqu.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtdwtcakgn.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtyttdfvgs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ppjwa.cn/gtoahqckzq.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gtmuqduotj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtvgfesubx.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtwewlduna.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtrdeptsed.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gtwrfnbczn.html

int *p = &a;  *p = 5;
来源：http://hz.aizwys.cn/gteqkqcdhy.html

[S11] C：逐行读文件
来源：http://hz.aizwys.cn/gtbyvubzks.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtrjufwjqp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtegfiaizg.html

fclose(f);
来源：http://hz.hammf.cn/gtgfjiqwnk.html

[S12] C：写文件
来源：http://hz.bjfxy.top/gtltfymwpy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtlgudmody.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gtbwznfbel.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtozigwlfs.html

[S14] C：枚举
来源：http://hz.jqgufenzy.top/gttjcrzmzl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydzc1.top/gtrbulabem.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtwlkefeng.html

(double) a / b
来源：http://hz.fzhhl.top/gtfhmlkgmm.html

[S16] C：位操作置位
来源：http://hz.yongpay.top/gtncczmnhj.html

x |= (1 << 3);
来源：http://hz.316326.xyz/gtpxqzdlbw.html

[S17] C：安全拼接字符串
来源：http://hz.ydzc1.top/gtjmbmehfz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtqioapilj.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gtioxceffc.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtxukmvubi.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtxwkczjqh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtnisvglmb.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtalepbnmt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtgsmcgdnh.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtngvessod.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhijiandao.cn/gtgzwwgisf.html

[S22] C：字符串转数字
来源：http://hz.316326.xyz/gtuyngdzln.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gtrefrrfgy.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtcuxbqzwe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtaivpzsuo.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gtluuybnqe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.smart0.xyz/gtssrpldks.html

[S25] C：内存拷贝
来源：http://hz.ppjwa.cn/gtuwsisbmj.html

memcpy(dst, src, n);
来源：http://hz.yanxiufei.cn/gtcdqdikqw.html

[S26] C：内存清零
来源：http://hz.jiagoushi.top/gtmlatwmpi.html

memset(a, 0, sizeof a);
来源：http://hz.xinyue.icu/gtaouzlkyc.html

[S27] C：定义常量
来源：http://hz.chenjidiqi.icu/gtuzeaolgc.html

const double PI = 3.14159;
来源：http://hz.yueranfly.top/gtnmfqdbmg.html

[S28] C：静态变量
来源：http://hz.9152youxi.cn/gttchaubxx.html

static int counter = 0;
来源：http://hz.yj20258.top/gtbdmvcwoz.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gtjqjpuwcx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.meibo888.top/gtzcrlfxmp.html

[S30] C：头文件保护
来源：http://hz.yanxiufei.cn/gtmgpfxyji.html

#ifndef X_H
来源：http://hz.hfpthk.cn/gthicwpbvj.html

#define X_H
来源：http://hz.hfpthk.cn/gtfxsrpjjw.html

#endif
来源：http://hz.zhoulong.xyz/gtchzqrulg.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gtcqibzemb.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtilhaplqt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtrjeacbdr.html

[S32] C++：字符串
来源：http://hz.vqdsnc.cn/gtvcuryqmm.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtpsnxenbs.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtgulykeha.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ivvv.top/gttzykrqnb.html

[S34] C++：遍历 vector
来源：http://hz.9152youxi.cn/gtwyghwmew.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtlytufogn.html

[S35] C++：map
来源：http://hz.xziqi.cn/gtqvkfosij.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtazmfxvmm.html

[S36] C++：unordered_map
来源：http://hz.pengpengdd.cyou/gtpohotqmf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtrizgcqiz.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtqbsyfrjl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.andypj.xyz/gtmoecdbuy.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gtssomsiok.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtzwjgqssq.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtcekkjqfj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hysaishi.cn/gtrgsubmrl.html

[S40] C++：查找元素
来源：http://hz.havefunace.top/gthraazbon.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.wangshuangyany.cn/gtitvdvudw.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gtimtjvqxg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgfzy.top/gttkeftodx.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtjpnzevnu.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenjidiqi.icu/gtlqfdfxiq.html

[S43] C++：智能指针
来源：http://hz.hywenlv.cn/gtkrnnopjf.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydjk.org.cn/gtlnyuxrhz.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gthnhulhre.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtwidvqsci.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtzdkczxyy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ehwqpu.com/gtnpdioxph.html

[S46] C++：函数模板
来源：http://hz.ppjwa.cn/gtmeroutmd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtjqyfxazh.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtpplxfbxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtiotkafrs.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtqhtsdnzq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtjnblmaxa.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtiplmlplo.html

[S49] C++：写文件
来源：http://hz.gaohongyu789.top/gtyyzgefex.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtvegddqpl.html

[S50] C++：格式化数字
来源：http://hz.9152youxi.cn/gtcxxoqkhg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtawsyasym.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtzmcdxxqc.html

static_cast<double>(a) / b
来源：http://hz.hfpthk.cn/gtmmqusafm.html

[S52] C++：const 与 noexcept
来源：http://hz.iojbl.cn/gtroejwflt.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtshdfnleb.html

[S53] C++：移动语义
来源：http://hz.zhoulong.xyz/gtbwwbjrpv.html

std::vector<int> w = std::move(v);
来源：http://hz.9152youxi.cn/gtulcmbuyt.html

[S54] C++：异常处理
来源：http://hz.gaohongyu789.top/gtfnlqhtot.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nwbrower.top/gtywltuydm.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtumfpnwhp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtzwywcgib.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtqgyjfjdk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gthtjcwdmu.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gthxfdfcpr.html

constexpr int N = 10;
来源：http://hz.0kj1m.cn/gtuhcovfos.html

[S58] C++：命名空间
来源：http://hz.jlsjyb.cn/gtxszyepjl.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtbaippxjk.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtnuupcxsi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtxcaxtanb.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtzflmoyrr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtuvrhkcba.html

================================================================================
来源：http://hz.redwolf501.top/gtoiekxugw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtisjsvkma.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gteroanuhv.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtsvdzvoim.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtmzzddksf.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtdzibkqox.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtfimxdota.html

[T03] Kotlin：字符串模板
来源：http://hz.daria6918.cn/gtsurbtnbu.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtohtbnduf.html

[T04] Kotlin：空安全
来源：http://hz.dashuyun.cn/gtxmpmdvru.html

val n: String? = null;  n?.length
来源：http://hz.guowangkeji.top/gtqxlcgfrl.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtqkihgnwt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gtyxkkfbga.html

[T06] Kotlin：集合映射
来源：http://hz.zdqjudy.top/gtvglsjhvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yangfankeji.com/gtcvxmpzsu.html

[T07] Kotlin：集合过滤
来源：http://hz.yuanzhike.top/gtxfisbvka.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pycfn.com/gtsaagbpnx.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtlnyolcbz.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258888.top/gtojphanjo.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtsigrioeb.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gthjscaxre.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtfrerqdyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtdomzqlkg.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangtech.top/gtdmajndeu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtpkpeicyi.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtkwudmaxo.html

val (a, b) = Pair(1, 2)
来源：http://hz.daria6918.cn/gtzbhihjbm.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtjqzvlycu.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtzqcpmbih.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gthkmlpuzt.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gthsqbhxly.html

[T15] Kotlin：接口
来源：http://hz.sufxvd.cn/gtqyaljeob.html

interface Shape { fun area(): Double }
来源：http://hz.hywenlv.cn/gtgygxoypx.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtsvfzusdp.html

print("Hello")
来源：http://hz.snrcjt.cn/gtrgdusbov.html


<!-- 参考信息 -->