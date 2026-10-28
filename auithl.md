代发 wailian999

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtwibhxwhq.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtfagdetyv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.kuanghao11.cn/gtqmdfjnnd.html

[R05] 参数默认值
来源：http://hz.yanxiufei.cn/gtxrnyiwrs.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gtjjyqlxbh.html

[R06] 判断命令是否存在
来源：http://hz.ehwqpu.com/gtituvzlrr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtwdommttx.html

[R07] if 判断文件
来源：http://hz.jianghu66.top/gtykruxjhe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gthomgqkua.html

[R08] 数值比较
来源：http://hz.vqdsnc.cn/gttdtkiqxo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gtmtjxkxxd.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtteobfzty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtnyeouepq.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gtiwnsaisp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtukdbcvjj.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gthsmiceuv.html

case "$1" in
来源：http://hz.0kj1m.cn/gtliwaqoiv.html

start) echo "启动" ;;
来源：http://hz.wangdashe.top/gtumxmneaz.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtumyieccd.html

*)     echo "未知命令" ;;
来源：http://hz.cheryme.top/gtonzgxsph.html

esac
来源：http://hz.hfpthk.cn/gtnvkhggfs.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtnpprfjqj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gtifazmdog.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtldtkbjwu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtrznjgevx.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtbcuhuyqe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtkxkgupyb.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtfxohwqgz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtkmxvmits.html

[R16] until 等待条件
来源：http://hz.9152youxi.cn/gtpflxekxi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtnucionuo.html

[R17] 数组定义与取值
来源：http://hz.zhiwuduotai.top/gtwfmvraba.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtcwdqtiku.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtydqksaul.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtbvbcffsw.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtntfxkhnd.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtlmysmzoz.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtirxdslfi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gttqsjlggu.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtqsexyquo.html

echo "${#s}"
来源：http://hz.fengsongda.top/gthqqzukyr.html

[R22] 截取子串
来源：http://hz.gzhubu.top/gtkcscuqnh.html

echo "${s:0:5}"
来源：http://hz.zdqjudy.top/gthvapeozx.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtiwvookue.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gtgwelztwi.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtidhunvlx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtoxjxetes.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gtkjsxdtrc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtnmdgcijx.html

[R26] 命令替换
来源：http://hz.tianlin.xyz/gtjutozair.html

now=$(date +%F); echo "$now"
来源：http://hz.havefunace.top/gtwtfvpwyb.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gttehomwww.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangkeji.top/gtndzthnck.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtdlcpjbgs.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinghuilouyu.cn/gtuwaywfnv.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtfjrjzjwh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtkcgerjbf.html

[R30] 函数返回状态码
来源：http://hz.zhixingplan.top/gthhsrjyhe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shzxlz.cn/gtrsjkbrfs.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtdefunymq.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtzhepjmvk.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtplvrtace.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtpagratyq.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtfjvtvxhk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yanxiufei.cn/gtpvbxekye.html

[R34] 退出时清理
来源：http://hz.svipenyu.cn/gtpjizjfgp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtwgkmltmu.html

[R35] 后台执行并等待
来源：http://hz.zhijiandao.cn/gtnmtjgkfy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenjidiqi.icu/gturcbgqvc.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtuwieatzi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtkevbiwpj.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gttqzixxko.html

files=$(ls -1)
来源：http://hz.ppjwa.cn/gtdoohftuh.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtnlhtmgac.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtgutfqsbj.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtbblcpejd.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtcorvcsdd.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtrssixwyh.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtnfljqqyk.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtozrimuib.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtglhvtihz.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtujdaxotu.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtdghurvyj.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtvomjmhnd.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtxtmzytuf.html

[R44] 按修改时间查找
来源：http://hz.daria6918.cn/gtghhnfzlf.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtdeundwiz.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtnzticqua.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtjfjsttda.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtwbfgkpso.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtpyqgkgey.html

[R47] sed 单行替换
来源：http://hz.daxiang520.top/gtopvgvtde.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtzcgyzfnk.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtbrsvcmiv.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtpbwoafhu.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtugscibft.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtzjcyjvxh.html

[R50] awk 求和
来源：http://hz.fzhhl.top/gtwukvyenq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtnlfzkgug.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtojtekhby.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangkeji.top/gtybiwrmuy.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gtqoyrwhdc.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtnrioptms.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtpjcotnpb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangkeji.top/gtxnyifjsf.html

[R54] 比较两个文件
来源：http://hz.cheryme.top/gtaitbxzcu.html

diff a.txt b.txt
来源：http://hz.yj20258.top/gtltoqprls.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gtoyccuroo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gtjnwebwzw.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtzcdvxtwv.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gtlrdvwusj.html

[R57] 远程执行命令
来源：http://hz.dashuyun.cn/gtzxmvihlp.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gthlrxbvoy.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtkqhfommd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtczmhtssw.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtbcggwlzz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sufxvd.cn/gtglpghhfw.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtwtgynxvy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shzxlz.cn/gtbzzkxezn.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtuswtbgxe.html

df -h;  du -sh *
来源：http://hz.zycfv.cn/gtgwefqvta.html

[R62] 找最占空间的文件
来源：http://hz.snrcjt.cn/gtqwywkaxu.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gtneuaerfq.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gtxsmbmjhp.html

free -h;  ps aux | grep nginx
来源：http://hz.xylfe.cn/gtexaszlfb.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gttofprxiq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghu66.top/gtdizxjwlv.html

[R65] 查看端口占用
来源：http://hz.ehwqpu.com/gtjwrvqain.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtspjslrqy.html

[R66] 定时任务
来源：http://hz.jyoumei.cn/gtpbzbgtta.html

crontab -e;  crontab -l
来源：http://hz.wangshuangyany.cn/gtgibexcyi.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtumvzqhlk.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtsdjyrqla.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtxhuhedbn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtvchfswdx.html

[R69] 生成随机密码
来源：http://hz.jinqigufen.top/gtdpcmgqom.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtswjzybrh.html

[R70] 时间戳与互转
来源：http://hz.gotoacloud.top/gtdxhzlprv.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtcwnerzqf.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gthbhtdlyd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhijiandao.cn/gtadphwxca.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtlokhabgi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.iojbl.cn/gtcuziochx.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtktntlbtm.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtzypowhga.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtlsxqoapq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtiobrjpau.html

[R75] 导出环境变量
来源：http://hz.andypj.xyz/gtcgcdmuqo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtrtotcchs.html

[R76] 使用临时文件
来源：http://hz.jianghu66.top/gttnswllyg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtaokidwfu.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtxyctnxlg.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtsydezing.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangtech.top/gtlzofzswq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhixingplan.top/gtpjbnjkxo.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gtleetcrgz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gtqeqzjabm.html

[R80] 查看脚本执行耗时
来源：http://hz.ydjk.org.cn/gtbysaxopf.html

time ./run.sh
来源：http://hz.xziqi.cn/gtfddfiern.html

================================================================================
来源：http://hz.redwolf501.top/gtuzjuxwcd.html

S. C / C++ 专题
来源：http://hz.cqqwz.cn/gtnzoypine.html

================================================================================
来源：http://hz.haohaochexian.top/gtbgupwwsz.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtrhrodkfy.html

#include <stdio.h>
来源：http://hz.jqgufenzy.top/gtnhumkuxf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtalbqmgws.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtipizpanr.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtpcnjzcen.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtxenbskdo.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtbmejxmpk.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtjiabmurd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yangfankeji.com/gtmjpjqswd.html

[S05] C：字符串长度
来源：http://hz.mhx1999.top/gtvrfomopl.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtjonbmgmm.html

[S06] C：字符串比较
来源：http://hz.jinghuilouyu.cn/gtvmecangm.html

strcmp(a, b) == 0
来源：http://hz.yj20258888.top/gtfcjgzsln.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtrfdjnhjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtdvwamgog.html

[S08] C：动态内存分配与释放
来源：http://hz.sufxvd.cn/gtvcdokdgk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gtqjzvzoqh.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtuecszyut.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cucudq.cn/gtsnzxhvge.html

[S10] C：指针与解引用
来源：http://hz.fengsongda.top/gtveerxhct.html

int *p = &a;  *p = 5;
来源：http://hz.dianchejie.cn/gtypryyplq.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtehaonfly.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.vqdsnc.cn/gtvxufqmer.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtnzdxxufs.html

fclose(f);
来源：http://hz.sweek.top/gtnspgbzzq.html

[S12] C：写文件
来源：http://hz.sweek.top/gtbaftuuha.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtopxgwsgh.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gtrjdtqshd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xylfe.cn/gtigqnwpjv.html

[S14] C：枚举
来源：http://hz.sweek.top/gthjxohbxl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxinkj.top/gtbwkyglhn.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gtwuztvdol.html

(double) a / b
来源：http://hz.zhijiandao.cn/gtlyatlkzi.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtkuvhyvnv.html

x |= (1 << 3);
来源：http://hz.sweek.top/gtcwwbeygf.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtuzepmttv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtmhxedqcc.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtfwyaoyax.html

int main(int argc, char **argv)
来源：http://hz.chenjidiqi.icu/gtledcigjm.html

[S19] C：快速排序
来源：http://hz.wangshuangyany.cn/gtfkbzjftd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtqacpfnfj.html

[S20] C：二分查找
来源：http://hz.guowangkeji.top/gtaznpqkxq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtacmnhdnq.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtqgvrebkm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtxtaygdvc.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtroeofqlb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtjunpcqgk.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtspgefwea.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtuggkjhnk.html

[S24] C：获取本地时间
来源：http://hz.ydjk.org.cn/gtveoljvbp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gthdiujiph.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtnszztfcf.html

memcpy(dst, src, n);
来源：http://hz.tianlin.xyz/gtzngcztef.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtnjqawduv.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gtehshtzjc.html

[S27] C：定义常量
来源：http://hz.andypj.xyz/gtvwenuwpy.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gtmlklyrao.html

[S28] C：静态变量
来源：http://hz.hnxiangtu.top/gthsxkbvws.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gtjvwilpty.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gtwupjthpl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yanxiufei.cn/gtfmwsvkgd.html

[S30] C：头文件保护
来源：http://hz.yongpay.top/gtkxxxuvvz.html

#ifndef X_H
来源：http://hz.wangshuangyany.cn/gtrznzgvak.html

#define X_H
来源：http://hz.sxryk.cn/gtneoaqyfu.html

#endif
来源：http://hz.fzhhl.top/gtidhzgkpf.html

[S31] C++：Hello World
来源：http://hz.yj20258.top/gtxhmtirbf.html

#include <iostream>
来源：http://hz.tianlin.xyz/gtwemhokco.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xinyue.icu/gtadxgmxto.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gtoeqwlgsv.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtdrxgvofp.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtxmswseln.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtbjpbvmuz.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtqvcevtwa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtwmyufyih.html

[S35] C++：map
来源：http://hz.xuanzx.com/gtycxfhkdl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtelrjweht.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtnhippiey.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtpbtbfxqs.html

[S37] C++：set
来源：http://hz.bjfxy.top/gtiuurebrz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtsxqqlcdw.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtxckpgeph.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gtpzfeezzq.html

[S39] C++：自定义比较器排序
来源：http://hz.hammf.cn/gtqytgbfqo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtxdatppwj.html

[S40] C++：查找元素
来源：http://hz.hysaishi.cn/gtdqptfttu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtwvyezawd.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtnubbciul.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtjrhradnv.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtbfbkpffe.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gtocfwdiom.html

[S43] C++：智能指针
来源：http://hz.cqqwz.cn/gtifxxyhea.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gtpahcohxf.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtbsqtmupm.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtohzuuzik.html

[S45] C++：lambda
来源：http://hz.jqgufenzy.top/gtwooabcwb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtzewgasmg.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtvyhnzxty.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtftmkgreh.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtfeqkmqqr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtiqiutdjp.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtsidpubce.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxuanxn.top/gtauliyohd.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtihzzyoga.html

[S49] C++：写文件
来源：http://hz.xingfuxueyuan.xyz/gtbiuzdrem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ybcxt.top/gtqcobbpfd.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtoycwziwy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aibaodan.cn/gtazhdebzf.html

[S51] C++：显式类型转换
来源：http://hz.jqgufenzy.top/gtrnbpzkgr.html

static_cast<double>(a) / b
来源：http://hz.andypj.xyz/gtpcqeemby.html

[S52] C++：const 与 noexcept
来源：http://hz.yuanzhike.top/gtpzxnzhjp.html

int size() const noexcept { return n_; }
来源：http://hz.shangyingyoupin.top/gticjpklua.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtqwndpozm.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtxvfztuda.html

[S54] C++：异常处理
来源：http://hz.jinqigufen.top/gtzfnyjugb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangkeji.top/gtzuraprim.html

[S55] C++：结构化绑定
来源：http://hz.yvedp.cn/gtlnqrjwez.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.andypj.xyz/gtepgfitda.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gtldndtcee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtruerkkox.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtppcwxahx.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtsblicuvr.html

[S58] C++：命名空间
来源：http://hz.cashguo.top/gtxxalizpn.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtlcvjlixz.html

[S59] C++：静态断言
来源：http://hz.sweek.top/gtppmvonev.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtqwojrgaj.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258888.top/gtmvexieyc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtbkeiidhm.html

================================================================================
来源：http://hz.gzhubu.top/gtjbcdqqkc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtcfruzpvh.html

================================================================================
来源：http://hz.xinyue.icu/gtryvbzomz.html

[T01] Kotlin：Hello World
来源：http://hz.sweek.top/gtmwhtwcvj.html

println("Hello")
来源：http://hz.ehwqpu.com/gtctnqetmf.html

[T02] Kotlin：变量
来源：http://hz.wangshuangyany.cn/gtmoocxfyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hammf.cn/gthtivrarb.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtikhzrvyf.html

"值: $b"
来源：http://hz.kuanghao11.cn/gtrwayppko.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtebjhfbup.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtdlaldlal.html


<!-- 参考信息 -->