代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gtlnympaot.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shzxlz.cn/gttiyhddyz.html

[Q83] 大小写转换
来源：http://hz.bjfxy.top/gtknrxulyo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.meibo888.top/gtqwvomkwo.html

[Q84] 去除首尾空格
来源：http://hz.c1oappe.top/gtglmtzncj.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtjynhilhj.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtnfwhueao.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xuetiantiany.cn/gtymauhcxv.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtwrztlgyl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtygahpztg.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtmidxazmj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xingfuxueyuan.xyz/gtkyypphry.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtinanwqph.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtkchlkezs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gttafmkuvf.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtyjpywptd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtbtehjixu.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtmcypqwjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtkdphmoet.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqkqrayxr.html

R. Bash 专题
来源：http://hz.yanxiufei.cn/gtdyuqkscp.html

================================================================================
来源：http://hz.gzhubu.top/gtxtktcdkb.html

[R01] shebang 与严格模式
来源：http://hz.svipenyu.cn/gtomgbnxkz.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtjumyvkpl.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtvkpxpwur.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtxisfizud.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtvagegmvx.html

[R03] 只读变量
来源：http://hz.sweek.top/gtrpwenldi.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtompoomcp.html

[R04] 位置参数
来源：http://hz.hammf.cn/gtmvywokur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gthivwyvpc.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtzxhkrqty.html

name="${1:-default}"
来源：http://hz.wangdashe.top/gtaoidbghv.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtyrhntivh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tanke756.top/gtphqlambz.html

[R07] if 判断文件
来源：http://hz.dianchejie.cn/gtbqiukkkl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtopeqbgez.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtwjbafkem.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258888.top/gtfozqmdtv.html

[R09] 字符串比较
来源：http://hz.zycfv.cn/gtwzaqpsey.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtjhkkjfrq.html

[R10] 正则匹配
来源：http://hz.mhx1999.top/gtzwovkzrs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtuavrzrmy.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gttlbaxpje.html

case "$1" in
来源：http://hz.gogol.net.cn/gtagcrupoz.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtrhothbsm.html

stop)  echo "停止" ;;
来源：http://hz.xziqi.cn/gtauznlrgv.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtctbwspqn.html

esac
来源：http://hz.zhijiandao.cn/gtvgjwnaeb.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtenmjigmn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtlsplmxij.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtzziwweal.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtxplvprow.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gtexgyggjs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtvrdjloyp.html

[R15] while 逐行读文件
来源：http://hz.jinqigufen.top/gtzbzxxrpr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yonumen.top/gtolzhuwaf.html

[R16] until 等待条件
来源：http://hz.sweek.top/gtwtfdckba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yonumen.top/gtfookjjyj.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtuiyixaqt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhiwuduotai.top/gtfysblnmk.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtdfdxodxr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtegzeiifd.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtumuxazws.html

echo "${#arr[@]}"
来源：http://hz.chenlongwang.top/gtebgssrkv.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtjqqibtrv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtaovrrngy.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtlyqclodl.html

echo "${#s}"
来源：http://hz.dashuyun.cn/gtftnxfegh.html

[R22] 截取子串
来源：http://hz.ydzc1.top/gtfjtnqznf.html

echo "${s:0:5}"
来源：http://hz.chenzaomai.com/gtcprkqanj.html

[R23] 字符串替换
来源：http://hz.cucudq.cn/gtihvdncmv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guannengcc.top/gtsrpgciku.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtlzffvkwq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guowangkeji.top/gtlipddrrn.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtnragwvfd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yangfankeji.com/gtwilmcsfy.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtyrfxrzji.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gtufhvsdaf.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtigbmmhxb.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtghpajsgi.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtjxjvfgnf.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtwgzmndof.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtxznjqrao.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.quarkkingdee.top/gtpplrifoo.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtwlxzfwfj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtqznkligp.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtvhrkplvs.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtqeeytunr.html

[R32] 参数个数校验
来源：http://hz.birdmap.top/gtslrqwkid.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtxoejtupd.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gtzbmqukbp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtlxbwsnxo.html

[R34] 退出时清理
来源：http://hz.nanxuanxn.top/gtlqnatali.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtaiyzzfkl.html

[R35] 后台执行并等待
来源：http://hz.jinyuanbaomall.cn/gtunjqbudb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gthszitjwf.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtisqbnxwg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtqmoypczi.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtfonszijp.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtoxmcyvob.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtkuxyrvos.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtjrnocgne.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtspzlkewn.html

cmd > out.log 2>&1
来源：http://hz.jlsjyb.cn/gtzjsfzwdz.html

[R40] 追加写日志
来源：http://hz.zhiwuduotai.top/gtbycvosbz.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gttmsqjumi.html

[R41] 丢弃输出
来源：http://hz.zhengqikj.top/gtesnibdpp.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtadkvelnu.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtixqfoxzk.html

wc -l < a.txt
来源：http://hz.mhx1999.top/gtxwbjjhel.html

[R43] 按名字查找文件
来源：http://hz.xylfe.cn/gtixtpwexh.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gttgoheqwz.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtkgrpgoat.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtqfbykaez.html

[R45] 批量删除
来源：http://hz.svipenyu.cn/gtqhiohvnq.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtdjjnyjvb.html

[R46] 递归替换文件内容
来源：http://hz.birdmap.top/gtakxyvewe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtibtawcox.html

[R47] sed 单行替换
来源：http://hz.jlsjyb.cn/gtdiaukvam.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gttedbwfvl.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtqpdlqdgw.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtagzzspsv.html

[R49] awk 带条件
来源：http://hz.shuidangran.top/gtywjyprqp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtvuwbgifs.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtscyiutdb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhoulong.xyz/gtnfxfcfyp.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtnuhfyxsq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sxryk.cn/gtujgdlyij.html

[R52] 统计行数
来源：http://hz.hnxiangtu.top/gtkucdakbw.html

wc -l a.txt
来源：http://hz.pycfn.com/gttutrldpr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhoulong.xyz/gtrmorktna.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtndzluncb.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gtolwldrmh.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gtfkrsizmp.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gtumcpficy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtgkmprehf.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtjtimphji.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtseadxilp.html

[R57] 远程执行命令
来源：http://hz.daxiang520.top/gthwhehmgp.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtkfvvpzyj.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtdbtpubnh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gtjenrinbt.html

[R59] 发 POST JSON
来源：http://hz.sufxvd.cn/gtqzpwactx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gtzygobkpj.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtigqqdvzo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtbfaprkjp.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gtskefhted.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtlktgplzm.html

[R62] 找最占空间的文件
来源：http://hz.jinyuanbaomall.cn/gtgbckrekn.html

du -ah . | sort -rh | head -10
来源：http://hz.tian-w.cn/gtywdnmrgy.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtlazafdvz.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigufen.top/gtccgiyxmb.html

[R64] 结束进程
来源：http://hz.hongshengwenyu.top/gtxgcjqurk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gttackgkzn.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gtkkvxackd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtuhecsfsk.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtpdyrbklt.html

crontab -e;  crontab -l
来源：http://hz.jqgufenzy.top/gthbduvcfw.html

[R67] 生成随机十六进制串
来源：http://hz.sufxvd.cn/gtpwjcdhth.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gttylkzwfw.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gttqkjwdik.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xziqi.cn/gttinvsnus.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtpzqvbkvu.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtjstzekrh.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtpkzefjmd.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gtwtaursnw.html

[R71] 日期格式化
来源：http://hz.dianchejie.cn/gtrmjfzqzr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.mhx1999.top/gtqatmagaw.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtekgltbqb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtelxdmeac.html

[R73] 分割大日志
来源：http://hz.snrcjt.cn/gtfcupcbcl.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gtsuamrqei.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtsgugewey.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtmjbpweai.html

[R75] 导出环境变量
来源：http://hz.jiagoushi.top/gtvvpaykwb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuanzx.com/gtpunwhcyp.html

[R76] 使用临时文件
来源：http://hz.yuxming.cn/gthafhysmb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtqcisznuz.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtkeacnelw.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtwzwfxojp.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtpsjdmtgn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtmyeybbor.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtvxwcbvyp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtifttejzi.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gthgttxqse.html

time ./run.sh
来源：http://hz.wangdashe.top/gtyyqiilnn.html

================================================================================
来源：http://hz.316326.xyz/gtkuaedkyp.html

S. C / C++ 专题
来源：http://hz.9152youxi.cn/gtwijiswbr.html

================================================================================
来源：http://hz.cheryme.top/gthxqhjwhy.html

[S01] C：Hello World
来源：http://hz.hnqzz.top/gtfptsypus.html

#include <stdio.h>
来源：http://hz.aibaodan.cn/gtnxmzpsxo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtpanbmhnk.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gtdfoawmvv.html

int a = 10; printf("%d\n", a);
来源：http://hz.gaohongyu789.top/gtdiluvikk.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtfchkplqu.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gtrfbfpkgf.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtfkcsvkuf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtabhypejs.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtczlnqoqi.html

strlen(s)
来源：http://hz.zhengqikj.top/gtfebkpxmg.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtbgqfhwnh.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtbekatrye.html

[S07] C：数组遍历求和
来源：http://hz.tianlin.xyz/gtakntswlu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtthtvsndf.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gtdyqtfrlj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gtfenglywg.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtagegtuxn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.haohaochexian.top/gtptktxalf.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gtyxaoapyw.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtgofkznev.html

[S11] C：逐行读文件
来源：http://hz.gaohongyu789.top/gteqflyqvi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtrbtwebpe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtwrmomphr.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtkkqypgly.html

[S12] C：写文件
来源：http://hz.sysykeji.top/gtsuraypyi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtjlvouumw.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtzpnbmihl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtajzxmcno.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtpgxwrzic.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gtfevdvafq.html

[S15] C：类型转换
来源：http://hz.svipenyu.cn/gtdepgodpe.html

(double) a / b
来源：http://hz.gogol.net.cn/gtwjlccpiy.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gthzgzrpjs.html

x |= (1 << 3);
来源：http://hz.zhoulong.xyz/gtwogwzdey.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtrsadmqfr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtzgjfsxmh.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtnpdwojsc.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtwaftlbta.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtrfvnzcpw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtxdizmrtx.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtydibjshs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtgpkbxbyi.html

[S21] C：字符类别判断
来源：http://hz.dashuyun.cn/gtlcpskajw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtgirvxvrd.html

[S22] C：字符串转数字
来源：http://hz.cdnleiting.top/gtktkdciny.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gttlglidvk.html

[S23] C：随机数
来源：http://hz.cheryme.top/gtnjhhhhdv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.iojbl.cn/gtojtiqpwh.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gtmpwltjry.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gzhubu.top/gthwzanhfu.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtzcgrgbyt.html

memcpy(dst, src, n);
来源：http://hz.sxryk.cn/gtzznwkjzy.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtqnqgcjdm.html

memset(a, 0, sizeof a);
来源：http://hz.jinyuanbaomall.cn/gtptiuxtul.html

[S27] C：定义常量
来源：http://hz.tianlin.xyz/gtaihlnhkp.html

const double PI = 3.14159;
来源：http://hz.daria6918.cn/gtyjqjzrct.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtnkbxxepb.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtpyuuxyjz.html

[S29] C：变参函数
来源：http://hz.xziqi.cn/gtuwyhthbp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtyupvzizy.html

[S30] C：头文件保护
来源：http://hz.vqdsnc.cn/gtozjhiplo.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtxthfdutb.html

#define X_H
来源：http://hz.gogol.net.cn/gtpqsjsmja.html

#endif
来源：http://hz.jqgufenzy.top/gtzxbbmyti.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtldpcfyoy.html

#include <iostream>
来源：http://hz.cdnleiting.top/gtuakcamxr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtdrbczimb.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtxxzikgfs.html

std::string s = "hi";  s += "!";
来源：http://hz.birdmap.top/gtmhqdtrcp.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtqwhklyqj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtedwnhzal.html

[S34] C++：遍历 vector
来源：http://hz.ydzc1.top/gtaniumtcp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxinkj.top/gttofbjqxp.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtbbxvuxdw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtopntzvye.html

[S36] C++：unordered_map
来源：http://hz.cucudq.cn/gtgkzxhtat.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtptrotdie.html

[S37] C++：set
来源：http://hz.havefunace.top/gtrdhuoieo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gtwmifnvfv.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gtunpnxnri.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtgpevfuie.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtnzljkhsb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangkeji.top/gtrkfjrdoa.html

[S40] C++：查找元素
来源：http://hz.ywan-chungtsiang.top/gtrmzluxea.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtzrbmiuui.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gtcsxtatip.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258.top/gtexicxnpm.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtqbkzuqkg.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gttjpwbkmx.html

[S43] C++：智能指针
来源：http://hz.sufxvd.cn/gtsdmhozfn.html

auto p = std::make_unique<int>(5);
来源：http://hz.redwolf501.top/gtfwgovlwl.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtojflibvx.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtmkhedanc.html

[S45] C++：lambda
来源：http://hz.zhongyouzk.top/gtbitymbiz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gotoacloud.top/gtigwebjkc.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gtlkwxiyos.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.meibo888.top/gtseffsmeb.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtczwdtrph.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tanke756.top/gtithcdosm.html

[S48] C++：逐行读文件
来源：http://hz.pycfn.com/gtilkwspqf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtdeywgitx.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtmfynlkre.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtdkhhtxve.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dashuyun.cn/gtcskfzmrb.html

[S50] C++：格式化数字
来源：http://hz.chenjidiqi.icu/gtuddznkkj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtnwhrkesi.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gteezczjos.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtnxsawhum.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtfwqdhenl.html


<!-- 参考信息 -->