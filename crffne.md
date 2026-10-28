代发 wailian999

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gtmwuugfwi.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtzqbkgvpu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtgqkkbsrr.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtyatthuir.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtyipwfvwf.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtghbzyawr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtorvnzvtm.html

[Q74] 强制使用索引
来源：http://hz.yonumen.top/gtikxditay.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.andypj.xyz/gtvcgfrtwi.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtlkplphtv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtzuaymlnf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.svipenyu.cn/gtthtzaomv.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gttwvtpgyg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtidffkrsq.html

[Q77] 时间加减
来源：http://hz.zhijiandao.cn/gtshfwshng.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtxvviqajk.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gtbrsajpvn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtgisudcfg.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtedekrdbz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gttjbdnvaz.html

[Q80] 字符串截取
来源：http://hz.hnqzz.top/gthgvwvwqt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxinkj.top/gtizeejtxt.html

[Q81] 字符串替换
来源：http://hz.nanxuanxn.top/gthuwyfcck.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ybcxt.top/gtceofarim.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtwabtwaqj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenjidiqi.icu/gthrcbaakm.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gtukdkxzkc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuanzx.com/gtdejchghu.html

[Q84] 去除首尾空格
来源：http://hz.hfpthk.cn/gtxapgsegp.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxinkj.top/gtjdvsgnza.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtqvmbsodu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj202588.top/gtrcqympux.html

[Q86] 读取 JSON 字段
来源：http://hz.hywenlv.cn/gtkyvafacm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtmvvbdxnv.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtaovblmxv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtvrdnfwwt.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtlbjqwpwl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangshuangyany.cn/gtwxwhpite.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gtirjvpcjp.html

[Q89] 判断表是否存在
来源：http://hz.haohaochexian.top/gtzjzrwvgy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yanxiufei.cn/gtivuthiox.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtxfylivuv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtjkholahb.html

================================================================================
来源：http://hz.tian-w.cn/gtltrmhuqp.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtxxbaaufi.html

================================================================================
来源：http://hz.shuidangran.top/gthomsbdxd.html

[R01] shebang 与严格模式
来源：http://hz.pengpengdd.cyou/gttbcrmkhb.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtcsumnysl.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtuqdfthbs.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtcvftnxnc.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtnirbrene.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtplxpmduh.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtwhddamxs.html

[R04] 位置参数
来源：http://hz.mhx1999.top/gtitmqsjni.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yangfankeji.com/gtiaxupsxa.html

[R05] 参数默认值
来源：http://hz.cucudq.cn/gtxbzoaxro.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gteapstlhu.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtagymumcx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtqjvlmqah.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtwplomwof.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtkuczefmg.html

[R08] 数值比较
来源：http://hz.wangdashe.top/gtjoggvuul.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtcgdtwhpc.html

[R09] 字符串比较
来源：http://hz.zhoulong.xyz/gtovninfir.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtqirydpet.html

[R10] 正则匹配
来源：http://hz.ydzc1.top/gteepurobe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ywan-chungtsiang.top/gtyfgfcphj.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtdswxsttq.html

case "$1" in
来源：http://hz.yj20258.top/gtnwialcjb.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gtzxazejhe.html

stop)  echo "停止" ;;
来源：http://hz.wangdashe.top/gtlomvwhvj.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtzamgrwat.html

esac
来源：http://hz.hysaishi.cn/gtpdztuywm.html

[R12] for 遍历文件
来源：http://hz.sufxvd.cn/gtaaqbheje.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuanzx.com/gthzhikcgp.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtchpyddbg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtpdcsixwp.html

[R14] C 风格 for
来源：http://hz.smart0.xyz/gtcqqfzuob.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtrikcyven.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtbezcgxyj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gtrrxbrvjd.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtgoddzmxu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenlongwang.top/gtybelgmpe.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtqtuohjhc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtxrsacrpn.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtlzrinbuv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtidydaeae.html

[R19] 数组长度
来源：http://hz.feifeiyinyue.top/gtasuukrmz.html

echo "${#arr[@]}"
来源：http://hz.hysaishi.cn/gtmijhoqgm.html

[R20] 关联数组（字典）
来源：http://hz.yangfankeji.com/gtobzfijme.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtpkmvpcsy.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gttkxjsfta.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtrwnulwgf.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtidlmxudc.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtdplspudj.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtljalkgxz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sysykeji.top/gtdvbqhxpf.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtmjyyiddf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtahwamlct.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtvaqqvqcc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtauvdpboh.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gthiilqiov.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtmdxgfygn.html

[R27] 算术展开
来源：http://hz.cqqwz.cn/gteyqgadfu.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtfxtdctco.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gttpwpoabd.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtzpchirof.html

[R29] 定义函数
来源：http://hz.316326.xyz/gtoiuipenf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hywenlv.cn/gtmrcsjnux.html

[R30] 函数返回状态码
来源：http://hz.ybcxt.top/gthxwengmy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtycdueiyk.html

[R31] 局部变量
来源：http://hz.meibo888.top/gtyyvaqzoq.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinghuilouyu.cn/gtuhioberq.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gtqesmdkyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sweek.top/gtozuubeec.html

[R33] 捕获错误并提示行号
来源：http://hz.feifeiyinyue.top/gtzetniuah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtpujykoyy.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtgfxjhdvt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtplwxvxyr.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtbjphdnnv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtxktpjmil.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtklogxdgd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydzc1.top/gtcblqpmvy.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gteltifysx.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtujgthfpd.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtkljcwmdk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinyuanbaomall.cn/gteuxalixl.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtmhkpfdjw.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtfwrrdffp.html

[R40] 追加写日志
来源：http://hz.wangdashe.top/gtwovcezbc.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtbilhkmfz.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtlzcrlxfm.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigfzy.top/gtlyuyjimi.html

[R42] 输入重定向
来源：http://hz.nwbrower.top/gtewhyvocw.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtmmfnsrze.html

[R43] 按名字查找文件
来源：http://hz.kuanghao11.cn/gtsittbivu.html

find . -name "*.log" -type f
来源：http://hz.tianlin.xyz/gtignkrtzg.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtwwsddhln.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtifrmhrol.html

[R45] 批量删除
来源：http://hz.yuanzhike.top/gtxslgbktj.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtnvwswhes.html

[R46] 递归替换文件内容
来源：http://hz.smart0.xyz/gtbzyjgnyd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ehwqpu.com/gtshsrknpi.html

[R47] sed 单行替换
来源：http://hz.zhoulong.xyz/gtcfkammpl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gttgyejojs.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtqihgbufc.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtemivrawo.html

[R49] awk 带条件
来源：http://hz.jianghu66.top/gtadfyvnav.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtioucldzo.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtgqbvsjxd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yanxiufei.cn/gtvumfydps.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gtytgnjgjk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gtjzbyjkrp.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtjytfyfet.html

wc -l a.txt
来源：http://hz.zhengqikj.top/gtivdvarlu.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gthiocaghw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtuowwbegr.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtrxwlqadj.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtvsdoyngc.html

[R55] 压缩与解压
来源：http://hz.yj202588.top/gtxcrvydwg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fengsongda.top/gttpmfmeqw.html

[R56] 远程拷贝
来源：http://hz.ehwqpu.com/gtgwnambie.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gthuzkymdo.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtiwkzjwpx.html

ssh user@host 'uptime'
来源：http://hz.fengsongda.top/gtutpqnkgx.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtancdddio.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dianchejie.cn/gtwhnpbggc.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtkuerdvbm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtsodlorjz.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtndfkfyys.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gthmajhqju.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gtciujpmwt.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtthtopcqy.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtoldmouvv.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtkjvgvihg.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gtnnfbskfg.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtquhhvuja.html

[R64] 结束进程
来源：http://hz.zycfv.cn/gtdpkjavqr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.mhx1999.top/gtuaqqrjgi.html

[R65] 查看端口占用
来源：http://hz.gzhubu.top/gtrvlefwve.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtrshhdomp.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtwteyhpuj.html

crontab -e;  crontab -l
来源：http://hz.guowangkeji.top/gttzgrcnem.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtenschqhv.html

openssl rand -hex 16
来源：http://hz.9152youxi.cn/gtkkdpitzv.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtfsoqixxo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtvrsppiqm.html

[R69] 生成随机密码
来源：http://hz.jinyuanbaomall.cn/gtofjpkscq.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtcajvodys.html

[R70] 时间戳与互转
来源：http://hz.xingfuxueyuan.xyz/gtzbhqvbyk.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtvatgrwvs.html

[R71] 日期格式化
来源：http://hz.shuidangran.top/gtnjicfxjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gtbuhsxogj.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtpuiehqop.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnqzz.top/gtmzsqbbdy.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtwlqycdzq.html

split -l 1000 big.log part_
来源：http://hz.cashguo.top/gtaqgfnzdv.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtlxnvhvkq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtngkydjzq.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtkfadhrii.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtyjhzohcw.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtjudwtamy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtvuuwmkql.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtzcyuvjib.html

read -rp "请输入: " ans
来源：http://hz.zycfv.cn/gtmuhfuasq.html

[R78] 交互式菜单
来源：http://hz.fengsongda.top/gtkbtefzdy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.feifeiyinyue.top/gtsjvgpcaz.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtjnhrvnkm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtglhzecen.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtodkfghcd.html

time ./run.sh
来源：http://hz.yangfankeji.com/gteangjvxx.html

================================================================================
来源：http://hz.cheryme.top/gtpdpjgucs.html

S. C / C++ 专题
来源：http://hz.9152youxi.cn/gtqsusurqh.html

================================================================================
来源：http://hz.svipenyu.cn/gtcebvrory.html

[S01] C：Hello World
来源：http://hz.guannengcc.top/gtfmcwhndv.html

#include <stdio.h>
来源：http://hz.sweek.top/gtccyeqsxh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shuidangran.top/gtpfulythd.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtwqzqwyam.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnqzz.top/gtbrlsezfc.html

[S03] C：读入整数
来源：http://hz.iojbl.cn/gtidjizins.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtnwmakvoj.html

[S04] C：字符串复制
来源：http://hz.hywenlv.cn/gtrqxqalzy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtbrysytmu.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtvorfemdu.html

strlen(s)
来源：http://hz.52xcode.cn/gtamjrkujb.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtccqtwrpu.html

strcmp(a, b) == 0
来源：http://hz.jinqigufen.top/gtwrmvnzab.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtjunuakil.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtlihdfftd.html

[S08] C：动态内存分配与释放
来源：http://hz.yuanzhike.top/gtphdlwcpo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenlongwang.top/gtwisxfofg.html

[S09] C：结构体定义与初始化
来源：http://hz.feifeiyinyue.top/gtlsjzqsyy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fengsongda.top/gtufkbobmh.html

[S10] C：指针与解引用
来源：http://hz.nwbrower.top/gtvsfarwqe.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtpvdgqetl.html

[S11] C：逐行读文件
来源：http://hz.sufxvd.cn/gtnobmxvoa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.316326.xyz/gtxhlqrdnf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgfzy.top/gtupinjjhy.html

fclose(f);
来源：http://hz.snrcjt.cn/gtlfpddkxj.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gtfluwgrbu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgfzy.top/gtlvkykuuj.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gtmfiorgxv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.vqdsnc.cn/gtazcyajhs.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtjwrkuqfk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhijiandao.cn/gtyqynkpbu.html

[S15] C：类型转换
来源：http://hz.wangshuangyany.cn/gtmvuhnfgo.html

(double) a / b
来源：http://hz.sxryk.cn/gtffopgwyt.html

[S16] C：位操作置位
来源：http://hz.xylfe.cn/gtyejdphfa.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtincuycif.html

[S17] C：安全拼接字符串
来源：http://hz.smart0.xyz/gtzlaskcuw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigfzy.top/gtimifjkvq.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtutxntetm.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangtech.top/gtaqmhazyc.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtkgrullgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtjximtjzo.html

[S20] C：二分查找
来源：http://hz.hfpthk.cn/gtibpxcgdu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gthxvqocga.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtyimavtow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tanke756.top/gtutgtodzg.html

[S22] C：字符串转数字
来源：http://hz.havefunace.top/gttmqejvyk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtxregygro.html

[S23] C：随机数
来源：http://hz.aizwys.cn/gtncwdvfwy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gteouxwjxh.html

[S24] C：获取本地时间
来源：http://hz.cqqwz.cn/gtqchhnnqc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nwbrower.top/gtedshkraq.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtvxzcrhnd.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtxfrbyylr.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gthvkkvdka.html

memset(a, 0, sizeof a);
来源：http://hz.shangyingyoupin.top/gtcpbrapoi.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtvfqlmnzx.html

const double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtgncyljwg.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gtvbdwxyda.html

static int counter = 0;
来源：http://hz.quarkkingdee.top/gtqzztatmg.html

[S29] C：变参函数
来源：http://hz.xuetiantiany.cn/gtrwdbomdg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtepnaitde.html

[S30] C：头文件保护
来源：http://hz.nanxuanxn.top/gteumtktju.html

#ifndef X_H
来源：http://hz.xuetiantiany.cn/gtwhigpyqw.html

#define X_H
来源：http://hz.hywenlv.cn/gtfghyidev.html

#endif
来源：http://hz.havefunace.top/gtrdwcoouj.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtrtkygmaq.html

#include <iostream>
来源：http://hz.yongpay.top/gtrlgpngvv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtdrmpmpnh.html

[S32] C++：字符串
来源：http://hz.vqdsnc.cn/gtavznnepb.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtbkbqtiqi.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtllbdpugc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.andypj.xyz/gtthcueoun.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gtptxvmwdx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtebwaowwt.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtcitvzzgm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtjsgqmlml.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gthapelmgj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtovemsktn.html

[S37] C++：set
来源：http://hz.shanyushiyangkeji.top/gtavxtjjeo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yongpay.top/gtqjvfrhtw.html

[S38] C++：排序
来源：http://hz.redwolf501.top/gtqjihzzqk.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gtcvowzgsk.html

[S39] C++：自定义比较器排序
来源：http://hz.yanxiufei.cn/gtxwvnnhwm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xylfe.cn/gtfatgklzv.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtigigonzd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gtmjsmolyj.html


<!-- 参考信息 -->