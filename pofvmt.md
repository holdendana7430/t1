代发 wailian999

[Q78] 当前时间
来源：http://hz.yonumen.top/gtlhroemyf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuetiantiany.cn/gtutnkxqdw.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtvgeidzve.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangtech.top/gtzkcwoycm.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtdkvnfnxi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hammf.cn/gtymlswfvo.html

[Q81] 字符串替换
来源：http://hz.hnqzz.top/gtrcokkhlw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtfduwulvh.html

[Q82] 字符长度与字节长度
来源：http://hz.chenzaomai.com/gtadvgtivb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtsfswmyxd.html

[Q83] 大小写转换
来源：http://hz.9152youxi.cn/gtyivbenbs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aibaodan.cn/gtxdnykjcm.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtktuigozy.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gthsxdbiqw.html

[Q85] 数值取整
来源：http://hz.vqdsnc.cn/gtoygzcfsv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtulnamivn.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtjfiootlc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jiagoushi.top/gtmeaddgdv.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtjlcubfpw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gturiszyrx.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gtlerqpjhh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gthznungxf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtdrbdhyya.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtiouscezx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.quarkkingdee.top/gttcwcyrbo.html

[Q90] 生成序号列
来源：http://hz.shuidangran.top/gtyedytprg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gthzmauscq.html

================================================================================
来源：http://hz.sysykeji.top/gtbxnwvpgx.html

R. Bash 专题
来源：http://hz.yj20258.top/gtkrtzmgpu.html

================================================================================
来源：http://hz.iojbl.cn/gtbtronrjz.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gthqgilxuz.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtchorgaik.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtpaspgtlj.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtvrzcjhav.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtoaswyxqo.html

[R03] 只读变量
来源：http://hz.0kj1m.cn/gtglscqqti.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtlsqhxzbd.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtzehdjztd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.feifeiyinyue.top/gtdtefynyy.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtjvymsqdq.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtlvtgncvx.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gtrizbiolh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtdqmqxyvc.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtpmosndzy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtdpxbvlva.html

[R08] 数值比较
来源：http://hz.vqdsnc.cn/gtrqhatuda.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yueranfly.top/gtqfbyfyrl.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtfvvlfdfv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtyhwasxnm.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtyzofdhsd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigfzy.top/gtgnswjtoi.html

[R11] case 多分支
来源：http://hz.yanxiufei.cn/gtyupcitgi.html

case "$1" in
来源：http://hz.jyoumei.cn/gtybknubdo.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gthldgwobu.html

stop)  echo "停止" ;;
来源：http://hz.hfpthk.cn/gtswwytmfq.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtbogwdpcv.html

esac
来源：http://hz.sysykeji.top/gtrauvmwma.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtvklxjrak.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtrpoxiqxl.html

[R13] for 计数循环
来源：http://hz.ydzc1.top/gtefcqajnl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hfpthk.cn/gtrswbdfym.html

[R14] C 风格 for
来源：http://hz.52xcode.cn/gtszghkljf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtehgtpiil.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gturjtblzm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ehwqpu.com/gtajeykaxa.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtkpnrtwff.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtxirwoojm.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gteqqlsbqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnxiangtu.top/gtclabkiks.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtbvxsakrb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.kuanghao11.cn/gtrmklpkoy.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtkvddjjrf.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtfhzmlxzn.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtbyojbbuv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xinyue.icu/gtrrwteuxu.html

[R21] 字符串长度
来源：http://hz.iojbl.cn/gtbxgnuiwh.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtgehkhfpm.html

[R22] 截取子串
来源：http://hz.shanyushiyangtech.top/gtlnkarjao.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtzvgxuyht.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtuggkzrek.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.redwolf501.top/gtrfotduss.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gtfhrfptme.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtbrgyhzkn.html

[R25] 去后缀 / 去前缀
来源：http://hz.xinyue.icu/gtiatharxd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cheryme.top/gtcigawqku.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtzhurwjuq.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gthafkgopu.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtfyoiuhck.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtfyurgtzz.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtwyefymfn.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gtllulwiyj.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtddmkfrbz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtskssrcal.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtblaenbhm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hywenlv.cn/gtfthgdxlr.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtjnbvndek.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtckuggxsg.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtjnjfmhnp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtbmcrzpuj.html

[R33] 捕获错误并提示行号
来源：http://hz.cdnleiting.top/gtraisddav.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtigqmxquq.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtftwcdcaq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtcwrfwxzg.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gtjkyehtdm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shzxlz.cn/gtqvyymafv.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtnwaaoooo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtannfqyze.html

[R37] 把输出赋给变量
来源：http://hz.zhoulong.xyz/gtefvakhis.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtuvzwjkmm.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gtdnnkucgb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtaartsjhc.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gthxdfmxqg.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtyqqolvsg.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtxlzgijey.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtxvlibjag.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtcnsksjli.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gthkcchuiy.html

[R42] 输入重定向
来源：http://hz.sweek.top/gtcwdbylol.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtoxomssxx.html

[R43] 按名字查找文件
来源：http://hz.0kj1m.cn/gtldwkwnfr.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtqoxpussf.html

[R44] 按修改时间查找
来源：http://hz.chenjidiqi.icu/gtzouadmmb.html

find . -mtime -7 -type f
来源：http://hz.xziqi.cn/gtbbbipnrh.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtzkfutpih.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtnykbpdju.html

[R46] 递归替换文件内容
来源：http://hz.hnqzz.top/gtjbqxyivd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtdwlkivjl.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gtrnqtynbn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhongyouzk.top/gtjerjbpmm.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtcwbewlfb.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtgvtyajth.html

[R49] awk 带条件
来源：http://hz.shuidangran.top/gtocbbatem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtbanpunlk.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtyfrdxuhv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtwsagrfka.html

[R51] 排序去重取前几
来源：http://hz.jqgfzy.top/gtgehspqlg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtnlkkdgoo.html

[R52] 统计行数
来源：http://hz.yvedp.cn/gtkncmkjta.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtkbzuodab.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gthtdkkugw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hongshengwenyu.top/gtphrkfbuf.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtfhoxhshv.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtjdtkuzcw.html

[R55] 压缩与解压
来源：http://hz.ivvv.top/gtvhplmijy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtqpnmlbwn.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtsweoyyuy.html

scp file user@host:/path/
来源：http://hz.yj202588.top/gtnrrgxiku.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtdyhulpgq.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtrtupmepi.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtebcaeklj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuetiantiany.cn/gtygxyyxrr.html

[R59] 发 POST JSON
来源：http://hz.zhongyouzk.top/gtuaksjbwm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gttxuosvxt.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtrqjrdtle.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtvxeckvbh.html

[R61] 磁盘占用
来源：http://hz.birdmap.top/gtaninpchc.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gtcpqdogvp.html

[R62] 找最占空间的文件
来源：http://hz.zdqjudy.top/gtbuatjnru.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtxkzdmccf.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gtmupwuaoo.html

free -h;  ps aux | grep nginx
来源：http://hz.hnxiangtu.top/gthodlykzz.html

[R64] 结束进程
来源：http://hz.sweek.top/gtaqlwcudr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtbilzuuwk.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtogucsefv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gtgnvjsluq.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gtjooubfrx.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gtulsnfmws.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gtgsnhkyfh.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtcevptzuc.html

[R68] 计算文件校验值
来源：http://hz.ywan-chungtsiang.top/gtugdfesbo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtrmvctcmw.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtiomucoef.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gthngaeonm.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtwlwqndhl.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gtcnwbdurx.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtbpfkthvn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtlgdtndvs.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtochsqqin.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgfzy.top/gtrvlwpqqr.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gtelslooqr.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtlkvcaayq.html

[R74] 批量重命名
来源：http://hz.yuxming.cn/gtratektmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinghuilouyu.cn/gtpqyukhfc.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtdteyoxud.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yongpay.top/gtukcinkmb.html

[R76] 使用临时文件
来源：http://hz.52xcode.cn/gtptputgxl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtkaqbwqjn.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtilxkplza.html

read -rp "请输入: " ans
来源：http://hz.nanxuanxn.top/gtuhupiwpq.html

[R78] 交互式菜单
来源：http://hz.birdmap.top/gtydmuanco.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtudmjpfru.html

[R79] 解析命令行选项
来源：http://hz.ybcxt.top/gtlbettbqw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj20258888.top/gtxdgrfhiu.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtroyatxqr.html

time ./run.sh
来源：http://hz.yj20258.top/gtubuoqhzd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtahgoipsf.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gtacrwgfty.html

================================================================================
来源：http://hz.chenlongwang.top/gtxlwuabla.html

[S01] C：Hello World
来源：http://hz.shanyushiyangtech.top/gtslhccykm.html

#include <stdio.h>
来源：http://hz.316326.xyz/gthmfwrtie.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yongpay.top/gtljncubkq.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtioqwjtjb.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtxtuiweaq.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtxygmiytv.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtuehvpkyi.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtzfdnmvvv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gtlthoysdq.html

[S05] C：字符串长度
来源：http://hz.zhengqikj.top/gtyuhyztkl.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtveefkrjx.html

[S06] C：字符串比较
来源：http://hz.gogol.net.cn/gtskvyonnb.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtlzxrysoy.html

[S07] C：数组遍历求和
来源：http://hz.jianghu66.top/gtmcfifnas.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtxagcjlez.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtefoabsxc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aizwys.cn/gtwdoxcqfm.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gtdxnioykl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtqwfdtafd.html

[S10] C：指针与解引用
来源：http://hz.shuidangran.top/gtaxrucqda.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtaxxkkodb.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtrynnwllx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xingfuxueyuan.xyz/gtiwhbggrx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gtawyrtcsz.html

fclose(f);
来源：http://hz.52xcode.cn/gtovmqtuqn.html

[S12] C：写文件
来源：http://hz.yuanzhike.top/gtfghnnnqx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhixingplan.top/gtnyzngkqk.html

[S13] C：宏定义
来源：http://hz.cucudq.cn/gtnwqdmwuu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtuypijmvg.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtamuxbjpt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gzhubu.top/gtxhpnbvrf.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtgdowylew.html

(double) a / b
来源：http://hz.yuxming.cn/gtbqtkllwm.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtxrywyvpf.html

x |= (1 << 3);
来源：http://hz.hammf.cn/gtxwxxsshb.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtncxtjdzm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhongyouzk.top/gtztyujlak.html

[S18] C：命令行参数
来源：http://hz.tianlin.xyz/gttbwcperx.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtvzyygwxd.html

[S19] C：快速排序
来源：http://hz.hywenlv.cn/gtdhuuzemv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtnmgugvzg.html

[S20] C：二分查找
来源：http://hz.ywan-chungtsiang.top/gtpjpbqgzf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtmdgeusez.html

[S21] C：字符类别判断
来源：http://hz.jqgufenzy.top/gtbxxzplna.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gttrlwsrbo.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtcuqaofph.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtlvdzuywl.html

[S23] C：随机数
来源：http://hz.xuetiantiany.cn/gtyuffxgav.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gttfsxdqdz.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtqrnawdoa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shuidangran.top/gtvoqyvaqd.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtcdsvfycn.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtxfzwzhig.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtrepivhxa.html

memset(a, 0, sizeof a);
来源：http://hz.zhaomingkeji.xyz/gtiykwzzrr.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtxsdftvqs.html

const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtyftnayjc.html

[S28] C：静态变量
来源：http://hz.bjfxy.top/gtvlqdjtqi.html

static int counter = 0;
来源：http://hz.jinqigfzy.top/gtnpwcrwcq.html

[S29] C：变参函数
来源：http://hz.xylfe.cn/gtisxtlnnl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ybcxt.top/gttynlfsbj.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtszqnlzcg.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gtasqoljnt.html

#define X_H
来源：http://hz.shzxlz.cn/gtvgpwzqps.html

#endif
来源：http://hz.chenjidiqi.icu/gtuijoilkv.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gtxkwrrlqe.html

#include <iostream>
来源：http://hz.gotoacloud.top/gtyuodmlis.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtclwbkwpv.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtsmcswbgl.html

std::string s = "hi";  s += "!";
来源：http://hz.wangshuangyany.cn/gtfzyovxvv.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gtaypidvej.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gzhubu.top/gtjcyeidrb.html

[S34] C++：遍历 vector
来源：http://hz.shzxlz.cn/gtffsqmnst.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.andypj.xyz/gtsgbfrfpx.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gturaytbrg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtroaqqkqh.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtuuexnsfq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtacijnosd.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtaqpobctu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gogol.net.cn/gtcbthxggl.html

[S38] C++：排序
来源：http://hz.shanyushiyangkeji.top/gtxnguuxvo.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtqkcrqosy.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtirpvvztz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hongshengwenyu.top/gtesjejvla.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gtrturncrw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gtpmfgtggr.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtdmtujgto.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cucudq.cn/gtoblafurl.html

[S42] C++：继承与虚函数
来源：http://hz.wangshuangyany.cn/gtjedzyjhx.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtxkydzenv.html

[S43] C++：智能指针
来源：http://hz.zhixingplan.top/gtxgbvhplc.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtuikxaxzm.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtynkybleq.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtliwassjs.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtbufkxdgf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenzaomai.com/gtjmitrlmr.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtniftboeq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtkqamtflg.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangshuangyany.cn/gtileszbcg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gtocpdozzs.html

[S48] C++：逐行读文件
来源：http://hz.zhiwuduotai.top/gtyaqzmlxc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gtmesfayhc.html


<!-- 参考信息 -->