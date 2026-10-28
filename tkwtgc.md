代发 wailian999

[Q80] 字符串截取
来源：http://hz.sweek.top/gtgnlblzyq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yonumen.top/gtjfdgmasv.html

[Q81] 字符串替换
来源：http://hz.tianlin.xyz/gtargitpkq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gtspkqfqhc.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtxdxxoncu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuxming.cn/gtnphfqjoh.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtszgpawyz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtgngsrzwc.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtehtcfxcw.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtunzfdwmn.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtsppgbdax.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtbgpkpzkc.html

[Q86] 读取 JSON 字段
来源：http://hz.yonumen.top/gthxyxfezr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtnvoxvpiz.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gtkkoolbni.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ivvv.top/gtjxcnmoll.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtslfcuanr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gthleuskji.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtrpbxfmod.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtpbvsmhlp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jiagoushi.top/gtwdtgsvye.html

[Q90] 生成序号列
来源：http://hz.smart0.xyz/gtfodiudyu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tian-w.cn/gtuexcxtdg.html

================================================================================
来源：http://hz.yuxming.cn/gtjyvyshom.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtezjdqbsb.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcynjvlbc.html

[R01] shebang 与严格模式
来源：http://hz.jinqigufen.top/gtpekbzvkl.html

#!/usr/bin/env bash
来源：http://hz.52xcode.cn/gtkebxoffi.html

set -euo pipefail
来源：http://hz.chenlongwang.top/gtidssnxby.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtalzwheop.html

name="Tom"; echo "$name"
来源：http://hz.sxryk.cn/gtbgkwhtcg.html

[R03] 只读变量
来源：http://hz.tanke756.top/gtuywuotcd.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtdgcjhtzs.html

[R04] 位置参数
来源：http://hz.hongshengwenyu.top/gtcwbypmhq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gtpfxojoim.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtvgqpppwj.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtoceksoiq.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtoqewpmyb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtyfoqullx.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtwpcdmqjf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtxcxgsyhw.html

[R08] 数值比较
来源：http://hz.birdmap.top/gtszudfgqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hammf.cn/gtulgbfhhg.html

[R09] 字符串比较
来源：http://hz.daria6918.cn/gtvghbcjvd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.52xcode.cn/gtlezuhyii.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtiqxcatgr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.redwolf501.top/gtbdnoezxt.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtfsgllxuy.html

case "$1" in
来源：http://hz.tanke756.top/gtbcsqxaqp.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtuzsdpteu.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gthlowcsfx.html

*)     echo "未知命令" ;;
来源：http://hz.jinyuanbaomall.cn/gtywbbxxlc.html

esac
来源：http://hz.ydjk.org.cn/gtwyvntdbe.html

[R12] for 遍历文件
来源：http://hz.aizwys.cn/gtnwetnxvd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtykiwyhqj.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtoynudouq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtqrgjmhxx.html

[R14] C 风格 for
来源：http://hz.redwolf501.top/gtvyrvzbku.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtdnkedwsd.html

[R15] while 逐行读文件
来源：http://hz.xuetiantiany.cn/gtunxaovci.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtplnrcbsh.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtldcglskz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtiezpjmrb.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gtpadxgbdb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtjcgclras.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gtdszzdhtb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinyuanbaomall.cn/gtleygbblh.html

[R19] 数组长度
来源：http://hz.birdmap.top/gtynjvvxqs.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtgbxoiovd.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtjbyoqoum.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtatovvnhm.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtgmssdjho.html

echo "${#s}"
来源：http://hz.hnxiangtu.top/gtasobxlxo.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gthzfybxlx.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtzluutlye.html

[R23] 字符串替换
来源：http://hz.daria6918.cn/gtktomuxuf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtjsmumuce.html

[R24] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtmpasikyg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtsbzagaiw.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtudazmymj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sysykeji.top/gtumhntkaq.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtsqgxvivf.html

now=$(date +%F); echo "$now"
来源：http://hz.zhaomingkeji.xyz/gtmsntvaxn.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtnywjrxyl.html

echo $((1 + 2 * 3))
来源：http://hz.shuidangran.top/gtcxlugmpl.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtmhwyrngh.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gtubfhfwwi.html

[R29] 定义函数
来源：http://hz.shangyingyoupin.top/gtkatiaxft.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zycfv.cn/gtjbxipcpa.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gtuwrrmrys.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shuidangran.top/gtxcmfzyku.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtotzlpuer.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtdwwapjzr.html

[R32] 参数个数校验
来源：http://hz.wangshuangyany.cn/gtusyrjzai.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtrbyavpdl.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtghpwwelb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtdapjxjpc.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtohbkndch.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtpapsgfyo.html

[R35] 后台执行并等待
来源：http://hz.redwolf501.top/gtdntqqwbt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhiwuduotai.top/gtcodzcrha.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtfgifxtrn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtwqtavlen.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtwjhlbqis.html

files=$(ls -1)
来源：http://hz.shanyushiyangtech.top/gtetxzslab.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtravvuoce.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gttggvxztj.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtoishahea.html

cmd > out.log 2>&1
来源：http://hz.tianlin.xyz/gtcrmswwqf.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtrrgmkgar.html

echo "log" >> out.log
来源：http://hz.aibaodan.cn/gtugqjzqak.html

[R41] 丢弃输出
来源：http://hz.ydzc1.top/gtsimeqcsq.html

cmd >/dev/null 2>&1
来源：http://hz.hywenlv.cn/gtlnbixmrh.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtbevoqgwd.html

wc -l < a.txt
来源：http://hz.shangyingyoupin.top/gtfgrdurte.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtoodkggum.html

find . -name "*.log" -type f
来源：http://hz.chenlongwang.top/gthlmswgtx.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtfxblfzra.html

find . -mtime -7 -type f
来源：http://hz.daxiang520.top/gttalnyzaj.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtiwoeetmo.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtflccoief.html

[R46] 递归替换文件内容
来源：http://hz.haohaochexian.top/gtliwbdypt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtnuwbcthp.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtyqxtnssf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtxemkhpgc.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtckryrlxy.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtjzmwrszi.html

[R49] awk 带条件
来源：http://hz.jiagoushi.top/gtdxhtntcy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtfwushues.html

[R50] awk 求和
来源：http://hz.mhx1999.top/gtzfiierqw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtmffwqvca.html

[R51] 排序去重取前几
来源：http://hz.cashguo.top/gtcoxyuqtt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xinyue.icu/gtilwychbz.html

[R52] 统计行数
来源：http://hz.cdnleiting.top/gtxwshrwla.html

wc -l a.txt
来源：http://hz.yj202588.top/gtjivaghcs.html

[R53] 查看文件头与实时尾
来源：http://hz.shangyingyoupin.top/gtmtjjhfge.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xinyue.icu/gtrfseukku.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtxttibolk.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtiuroqkuu.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtoemvnack.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtdzlkgyjr.html

[R56] 远程拷贝
来源：http://hz.sysykeji.top/gtwxtyyzoi.html

scp file user@host:/path/
来源：http://hz.jyoumei.cn/gtlvcohxou.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtjxfaenvx.html

ssh user@host 'uptime'
来源：http://hz.fzhhl.top/gtnbgjexta.html

[R58] 下载文件
来源：http://hz.cdnleiting.top/gtsrxowxvq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtfxjtpoku.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtzdgwzwiz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jiagoushi.top/gtfddkpjss.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gticqdnpow.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gtvkvlnzym.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtzvykvcju.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtkgtrhtbp.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gtynmslgjq.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtspbvcbmt.html

[R63] 内存与进程
来源：http://hz.hnxiangtu.top/gtmjokatsy.html

free -h;  ps aux | grep nginx
来源：http://hz.chenzaomai.com/gtaegwszkp.html

[R64] 结束进程
来源：http://hz.jlsjyb.cn/gtmbmuthdx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhoulong.xyz/gtqimqagui.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtcgvoizlo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.316326.xyz/gtldurfxku.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtyzfhxdwf.html

crontab -e;  crontab -l
来源：http://hz.jinqigfzy.top/gtdbfzyjvt.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtlqvcbuwd.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtxpudqnwr.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtegpxqbum.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtorgtvksw.html

[R69] 生成随机密码
来源：http://hz.nwbrower.top/gtymfomruc.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinyuanbaomall.cn/gtomnrfsha.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtlqebulga.html

date +%s;  date -d @1700000000
来源：http://hz.andypj.xyz/gtrxvomoby.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtrnfhndfl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtovnrkdto.html

[R72] 等待端口就绪
来源：http://hz.0kj1m.cn/gtkaifllqz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtftossofw.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gtfvxsjbyb.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtoaeqyuqu.html

[R74] 批量重命名
来源：http://hz.ybcxt.top/gtbhmrwawj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yangfankeji.com/gttzuhyaie.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtltcwymob.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtnbkoaefs.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtsleuecri.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtiykzxmkf.html

[R77] 读取用户输入
来源：http://hz.hysaishi.cn/gtcgrugjdv.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtxonrzoyu.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtqxzukcfx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtsrwkcbuq.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtzxbipjgh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gtpufzjzqh.html

[R80] 查看脚本执行耗时
来源：http://hz.yuanzhike.top/gtnmzdecsn.html

time ./run.sh
来源：http://hz.shuidangran.top/gtblzgekcz.html

================================================================================
来源：http://hz.chenlongwang.top/gtvlhjkgof.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtqjsfmczk.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtyfdbiawa.html

[S01] C：Hello World
来源：http://hz.shanyushiyangkeji.top/gtctosjasq.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtvwewypbg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhengqikj.top/gthozitydc.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtqmhibbkl.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtpbxkqwhn.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtchtiwhxh.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtrwjxlnwf.html

[S04] C：字符串复制
来源：http://hz.guannengcc.top/gtovlcyaki.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtjevnhces.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtcmneluvr.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtuuttfoog.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtitltzsbe.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtfysxbuqf.html

[S07] C：数组遍历求和
来源：http://hz.jinqigfzy.top/gtwkjfwoyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhongyouzk.top/gtlcrrecdw.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtajgswsca.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ppjwa.cn/gtrxkaospy.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gttntxgtyh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yongpay.top/gtsevrcgav.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtirlqiohz.html

int *p = &a;  *p = 5;
来源：http://hz.jianghu66.top/gtpvgivbhy.html

[S11] C：逐行读文件
来源：http://hz.hfpthk.cn/gtuoqrwtas.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtpmsughuw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtendttszt.html

fclose(f);
来源：http://hz.hammf.cn/gtrheivhzz.html

[S12] C：写文件
来源：http://hz.sufxvd.cn/gtvorfvyqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtthvjfkox.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gttqhnjnzq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cashguo.top/gtrhtguzai.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtdjslbgfa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gtaqupijsc.html

[S15] C：类型转换
来源：http://hz.smart0.xyz/gtquvzzwjx.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtnutrdvkn.html

[S16] C：位操作置位
来源：http://hz.wangshuangyany.cn/gtummxfnog.html

x |= (1 << 3);
来源：http://hz.jianghu66.top/gtuduakinw.html

[S17] C：安全拼接字符串
来源：http://hz.meibo888.top/gtiykxgymn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gtdygoriuj.html

[S18] C：命令行参数
来源：http://hz.haohaochexian.top/gtqlbvqcir.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtsqbevkax.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gtswoobxwc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtjnklndyv.html

[S20] C：二分查找
来源：http://hz.ivvv.top/gtcololxfs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtylqfvene.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtldskugvf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.smart0.xyz/gtbznvulof.html

[S22] C：字符串转数字
来源：http://hz.hnqzz.top/gttcetqwbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gteoppdgrj.html

[S23] C：随机数
来源：http://hz.yvedp.cn/gtfrxthbnn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.aizwys.cn/gtplvqkifp.html

[S24] C：获取本地时间
来源：http://hz.gogol.net.cn/gtwfoooynq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtqxagmepd.html

[S25] C：内存拷贝
来源：http://hz.jinqigufen.top/gtajryhhnn.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtijrxddse.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gthtblrutv.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gthjwvvekd.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtxacvctpx.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gttyrlfmrb.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtldotcimb.html

static int counter = 0;
来源：http://hz.gotoacloud.top/gtgztefbwv.html

[S29] C：变参函数
来源：http://hz.ivvv.top/gtuhkvagtj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtuhbisiim.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtigxydnra.html

#ifndef X_H
来源：http://hz.haohaochexian.top/gtikowzuff.html

#define X_H
来源：http://hz.zhixingplan.top/gtegqfnsfu.html

#endif
来源：http://hz.bjfxy.top/gtumttjoab.html

[S31] C++：Hello World
来源：http://hz.shuidangran.top/gtltjdxyuj.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtcbgtpjjr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtdronluzb.html

[S32] C++：字符串
来源：http://hz.pengpengdd.cyou/gthkfjjdjl.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangkeji.top/gtdmhatono.html

[S33] C++：vector 增删
来源：http://hz.gotoacloud.top/gtqzdvhlzq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtslzbmkrv.html

[S34] C++：遍历 vector
来源：http://hz.yuanzhike.top/gthcolnvgr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.meibo888.top/gtxfgktqbz.html

[S35] C++：map
来源：http://hz.zycfv.cn/gtugsjghlg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtlsxjzhax.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtonaritsv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gteuuppdja.html

[S37] C++：set
来源：http://hz.cqqwz.cn/gtdpteyjhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gteuakihwd.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtqxndevhd.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtnsfnqhks.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtqjfspbsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtlzykhinh.html

[S40] C++：查找元素
来源：http://hz.jiagoushi.top/gtqgfbktte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtummztwnl.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtrocdvfsi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinghuilouyu.cn/gtbkqzcmcu.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtlogmdfoc.html

class B : public Base { public: void f() override {} };
来源：http://hz.cheryme.top/gtgqhubvlj.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtqzgogmhg.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtcscpvthv.html

[S44] C++：引用传参
来源：http://hz.gogol.net.cn/gtthvfuuza.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtslnlolrh.html

[S45] C++：lambda
来源：http://hz.quarkkingdee.top/gtersuymdj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtcwhwifmn.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtfjdrdfxc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.meibo888.top/gtkazchoyz.html

[S47] C++：结构化绑定遍历
来源：http://hz.feifeiyinyue.top/gtceftuzsh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuanzhike.top/gtbrxfzggv.html

[S48] C++：逐行读文件
来源：http://hz.yuxming.cn/gtyyisrryc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtsjfmwfjx.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtsoscanms.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtlyteskwc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtghcxprav.html

[S50] C++：格式化数字
来源：http://hz.hongshengwenyu.top/gtqziyadxt.html


<!-- 参考信息 -->