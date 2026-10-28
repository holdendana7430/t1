代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.pengpengdd.cyou/gtdmlrhdie.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtqxhnvwzm.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gtfeqiaini.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtxlrbutyd.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gttwyooauz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gtuwtkctyy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cdnleiting.top/gtfbsmxxwm.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtsyjdwxvj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtefpexgkm.html

[Q90] 生成序号列
来源：http://hz.cdnleiting.top/gtijcjwfsh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jyoumei.cn/gtanpfbkmi.html

================================================================================
来源：http://hz.dianchejie.cn/gtwjikwves.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtxwwufkfz.html

================================================================================
来源：http://hz.svipenyu.cn/gtkfecamkz.html

[R01] shebang 与严格模式
来源：http://hz.chenjidiqi.icu/gtmbeyebvy.html

#!/usr/bin/env bash
来源：http://hz.sweek.top/gtfdrvlxgx.html

set -euo pipefail
来源：http://hz.tian-w.cn/gtsicomuyv.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtvpocvfcm.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtetdxlkmt.html

[R03] 只读变量
来源：http://hz.kuanghao11.cn/gtuyxxsqlo.html

readonly PI=3.14
来源：http://hz.hnxiangtu.top/gttvwhnwsa.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtbarrugfw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gtdxpnxxju.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gtqzshpxet.html

name="${1:-default}"
来源：http://hz.chenjidiqi.icu/gtelpdmsyx.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtymqawyxd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtnsknzjjg.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtldhcctlg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shangyingyoupin.top/gtqvqwqknp.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtpgucembn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtawszlavj.html

[R09] 字符串比较
来源：http://hz.yongpay.top/gtiznbknqc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.quarkkingdee.top/gtbyihlxls.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtbgxtwymh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtfzlrdeum.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtexhihzqw.html

case "$1" in
来源：http://hz.redwolf501.top/gtcftachty.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtbflnecoq.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtdrtedkou.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtzvczqrzb.html

esac
来源：http://hz.nanxinkj.top/gtsreetatt.html

[R12] for 遍历文件
来源：http://hz.fzhhl.top/gtudvvmzto.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtehdtbwlh.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtrsvbqvjh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtdshaicfc.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtohdgpxti.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtdzkzoczy.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtlomhyvel.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtbmpwndra.html

[R16] until 等待条件
来源：http://hz.chenzaomai.com/gtzveecsft.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtpqidshjr.html

[R17] 数组定义与取值
来源：http://hz.guannengcc.top/gtvpltewpe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zdqjudy.top/gtmultfviv.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtxifdxnkz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.vqdsnc.cn/gtnyyecjqh.html

[R19] 数组长度
来源：http://hz.jlsjyb.cn/gtudhzkolr.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangtech.top/gthwaqygpz.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtukbhdhqz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gtrmtxrevi.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtpqubdqlz.html

echo "${#s}"
来源：http://hz.cqqwz.cn/gtmovnmmey.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtviptdphr.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtnsopjwkx.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gtqbpyqecj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtvenyrkhk.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtywqbnxla.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinghuilouyu.cn/gtbjyirwdu.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtwehfxpez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnqzz.top/gtdehcljor.html

[R26] 命令替换
来源：http://hz.gaohongyu789.top/gtpdufwfkj.html

now=$(date +%F); echo "$now"
来源：http://hz.havefunace.top/gtdmnzrwew.html

[R27] 算术展开
来源：http://hz.chenlongwang.top/gtuetchism.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gtpmuwzuea.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtyhnmfrxv.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuxming.cn/gtrscguyaa.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gteyfvbxdi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtwqwvadba.html

[R30] 函数返回状态码
来源：http://hz.smart0.xyz/gtykpmykyr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtyjsrlrdy.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtczezykvb.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtxifrwvvw.html

[R32] 参数个数校验
来源：http://hz.haohaochexian.top/gtunwymzku.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tanke756.top/gtzzydqngr.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtvdzhzzpk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yueranfly.top/gtlwhijmxr.html

[R34] 退出时清理
来源：http://hz.316326.xyz/gtsgfqmpck.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtuyvceenm.html

[R35] 后台执行并等待
来源：http://hz.ywan-chungtsiang.top/gtdjthmkyf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenlongwang.top/gtmzbscfud.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtiwwavwtn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fzhhl.top/gtpggwdsmf.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gttdwmrplx.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtwexraiks.html

[R38] 管道串联
来源：http://hz.hammf.cn/gtdubxrukz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gtzcufwmvi.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtlkxdjxgs.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gtbfgrxods.html

[R40] 追加写日志
来源：http://hz.kuanghao11.cn/gtmqdqyeen.html

echo "log" >> out.log
来源：http://hz.0kj1m.cn/gtcifqxhka.html

[R41] 丢弃输出
来源：http://hz.zhengqikj.top/gtlapidgne.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gthdoefibm.html

[R42] 输入重定向
来源：http://hz.feifeiyinyue.top/gtibvippmh.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtlbzjxwad.html

[R43] 按名字查找文件
来源：http://hz.yuanzhike.top/gtwawofgvx.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtkvapsrut.html

[R44] 按修改时间查找
来源：http://hz.c1oappe.top/gtdscexkng.html

find . -mtime -7 -type f
来源：http://hz.jiagoushi.top/gthpsigaop.html

[R45] 批量删除
来源：http://hz.hysaishi.cn/gtebzbbeod.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtatujiqge.html

[R46] 递归替换文件内容
来源：http://hz.daxiang520.top/gttrzlctcq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtlzurpnwp.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtfugdhibl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gtysitdbmz.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtwauaqopq.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnxiangtu.top/gtbytpumhc.html

[R49] awk 带条件
来源：http://hz.hywenlv.cn/gtetjxjkmg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtfuljrouz.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtiluvgurd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yongpay.top/gtmveeitum.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gttdpmqhbl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtvkovdhku.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtbxcodmfk.html

wc -l a.txt
来源：http://hz.yonumen.top/gtraozbsdf.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtqtjerves.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yanxiufei.cn/gtsnlwuppl.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtkbmjrchu.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gtjgilknbk.html

[R55] 压缩与解压
来源：http://hz.iojbl.cn/gtbdruschw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtoupeuffs.html

[R56] 远程拷贝
来源：http://hz.chenjidiqi.icu/gtepzisune.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtoaznnnlc.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtbwdwcfdw.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtopwlniar.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtolxcbkhl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtqdtqifjc.html

[R59] 发 POST JSON
来源：http://hz.zycfv.cn/gthdjnfnbo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtbxfhdfuh.html

[R60] 只看 HTTP 状态码
来源：http://hz.haohaochexian.top/gtgmhuoxqd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtxpquxeqw.html

[R61] 磁盘占用
来源：http://hz.hongshengwenyu.top/gtrsntcctq.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtogprromj.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtbhvvhzva.html

du -ah . | sort -rh | head -10
来源：http://hz.jiagoushi.top/gtzuqrpisc.html

[R63] 内存与进程
来源：http://hz.ybcxt.top/gtgajcfdod.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtjehrotwp.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtmywlskld.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhoulong.xyz/gtqperliux.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gtnkuwpool.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtlkqykhqd.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtguhhacgq.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtuygfxphc.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258.top/gtcutswqtp.html

openssl rand -hex 16
来源：http://hz.gaohongyu789.top/gtsmjdhyea.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtehcwustw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinyuanbaomall.cn/gttkfmzyeq.html

[R69] 生成随机密码
来源：http://hz.nanxinkj.top/gtafzqzudc.html

head -c 16 /dev/urandom | base64
来源：http://hz.c1oappe.top/gtztbljxey.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtknmzgvhp.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtdfknlnii.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtuzlvdewj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtvmzyhxqk.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gtnkdgwhcy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtezizwefo.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtvhccqsgo.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gtffvkfrme.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtbucnpxga.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtwlafbkrv.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gtgtwmpzzm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gthsqnlhvy.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtcjtcffpd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtuhwajqel.html

[R77] 读取用户输入
来源：http://hz.jqgfzy.top/gthtkxhdtm.html

read -rp "请输入: " ans
来源：http://hz.hongshengwenyu.top/gtjnomvmio.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtmpxuwmvf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtpvflyzkh.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtovkoyqom.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dashuyun.cn/gttuuxrtpf.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gttljpyecq.html

time ./run.sh
来源：http://hz.zhiwuduotai.top/gthiesvpyi.html

================================================================================
来源：http://hz.yuanzhike.top/gtemxgpmnm.html

S. C / C++ 专题
来源：http://hz.haohaochexian.top/gtymutaujs.html

================================================================================
来源：http://hz.haohaochexian.top/gteklyrfzp.html

[S01] C：Hello World
来源：http://hz.yuanzhike.top/gtmnoflcdj.html

#include <stdio.h>
来源：http://hz.daria6918.cn/gttqracrnl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tianlin.xyz/gtdrmbkhbe.html

[S02] C：变量与格式化输出
来源：http://hz.cashguo.top/gtyuvyapcu.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gtbnuqfozz.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtqoxuajow.html

int x; scanf("%d", &x);
来源：http://hz.cqqwz.cn/gtuijonzbt.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtijbsadea.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtfvumwulc.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtgluovzpd.html

strlen(s)
来源：http://hz.316326.xyz/gtjwtxexan.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtpkgllhib.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtltdsjjah.html

[S07] C：数组遍历求和
来源：http://hz.zhoulong.xyz/gtytkozbgr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ppjwa.cn/gtjpdfaooq.html

[S08] C：动态内存分配与释放
来源：http://hz.xinyue.icu/gtiuqtrcqt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtqjjyoiic.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtrjhgquaf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aibaodan.cn/gtpuogdill.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gthjjrlqsq.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gthkgkuozq.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtgxrhzifx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuxming.cn/gtxvhxkyxr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zycfv.cn/gtzesocuvx.html

fclose(f);
来源：http://hz.hywenlv.cn/gtbiibojuj.html

[S12] C：写文件
来源：http://hz.chenlongwang.top/gtuocwvvdv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gterlsepjz.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gthejlfjph.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtlwhskmyn.html

[S14] C：枚举
来源：http://hz.hnxiangtu.top/gtoeamqthv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtlcilmxxd.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtcrsyrxlk.html

(double) a / b
来源：http://hz.tian-w.cn/gtldejrjpb.html

[S16] C：位操作置位
来源：http://hz.ybcxt.top/gtgjiipjrw.html

x |= (1 << 3);
来源：http://hz.svipenyu.cn/gtmhnrfndp.html

[S17] C：安全拼接字符串
来源：http://hz.guowangkeji.top/gtpinoakyw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jlsjyb.cn/gtppkvbljh.html

[S18] C：命令行参数
来源：http://hz.cashguo.top/gtpfirgeid.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtpuenrnmd.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtlzfrinqk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtbadppaap.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtwpdnuyzj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtprtuzrqo.html

[S21] C：字符类别判断
来源：http://hz.gzhubu.top/gtcdhrlspy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtqmgcgaqw.html

[S22] C：字符串转数字
来源：http://hz.aizwys.cn/gtmhjshgbz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtpxyiypwx.html

[S23] C：随机数
来源：http://hz.hammf.cn/gttjihfwbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtoddfruzn.html

[S24] C：获取本地时间
来源：http://hz.wangshuangyany.cn/gtrgsetulm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangshuangyany.cn/gtsigelbme.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtsiitxcvp.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtkchansfl.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gtokalznzk.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gtcqzludpo.html

[S27] C：定义常量
来源：http://hz.nwbrower.top/gtyspdzrlv.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtvyomsvbt.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtmtoeywim.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtdxfhtmho.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtrljypgqm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cheryme.top/gtpufudrtm.html

[S30] C：头文件保护
来源：http://hz.fzhhl.top/gtctubajnv.html

#ifndef X_H
来源：http://hz.c1oappe.top/gthhrsnmdx.html

#define X_H
来源：http://hz.shuidangran.top/gtjlxrerlp.html

#endif
来源：http://hz.hnxiangtu.top/gtcpafrota.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtjvkrfpqs.html

#include <iostream>
来源：http://hz.yvedp.cn/gtibckwhqn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gtrnkvrjhd.html

[S32] C++：字符串
来源：http://hz.zhiwuduotai.top/gthzfouazt.html

std::string s = "hi";  s += "!";
来源：http://hz.kuanghao11.cn/gtcrjsgnib.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtgirtcsjh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dashuyun.cn/gtajqjwjmu.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtyxkzqzoh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtivbalxhl.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtgnbowwiw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtlljawauq.html

[S36] C++：unordered_map
来源：http://hz.hfpthk.cn/gtynazfbzd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtppuepsbv.html

[S37] C++：set
来源：http://hz.gotoacloud.top/gtnngmhtof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtcmfutefk.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtttxwdocg.html

std::sort(v.begin(), v.end());
来源：http://hz.jinqigfzy.top/gtwjmistdg.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gtemotciup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtndweazjz.html

[S40] C++：查找元素
来源：http://hz.pengpengdd.cyou/gthzqyxfjl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.kuanghao11.cn/gtvsgfwmbf.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtfupufvdl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gtwsqstcor.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtsheuwewa.html

class B : public Base { public: void f() override {} };
来源：http://hz.tanke756.top/gtgehopdms.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gtqpctueva.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gtihxrcunx.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtrhjpioef.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtphnynfpa.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gteuampjdq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtjdmlfwib.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtnayaowmz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guowangkeji.top/gtaslwlvjh.html

[S47] C++：结构化绑定遍历
来源：http://hz.mhx1999.top/gtojdlogvw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtlqrukirw.html

[S48] C++：逐行读文件
来源：http://hz.sufxvd.cn/gtynkkqrlp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtaqoxrsqc.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtmzohlqmy.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtizqnuetu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtgowjcmww.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtmtgqzzxm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gthtwgirzd.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtabgnzjgc.html

static_cast<double>(a) / b
来源：http://hz.ydjk.org.cn/gtignkumcy.html

[S52] C++：const 与 noexcept
来源：http://hz.yuanzhike.top/gtowdfxhvj.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtatfgqmdm.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtxnsviirj.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtllfhdfzk.html

[S54] C++：异常处理
来源：http://hz.cucudq.cn/gtxfhsqqoz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtwunpikqf.html

[S55] C++：结构化绑定
来源：http://hz.jqgufenzy.top/gttouhasbg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gtypjiigqp.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtxxpjoowb.html


<!-- 参考信息 -->