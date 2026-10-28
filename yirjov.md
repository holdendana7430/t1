代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aibaodan.cn/gtpiwammbm.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtqrqorrat.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gtphuytdby.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gttaoxtdxr.html

[Q76] 按天统计
来源：http://hz.jinyuanbaomall.cn/gtozxmvnhj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenjidiqi.icu/gtgmcpwifb.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtlvmumgfw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhengqikj.top/gtlvzkltos.html

[Q78] 当前时间
来源：http://hz.nanxinkj.top/gtelutrygq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtdfivbwmx.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtaaouiypm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.quarkkingdee.top/gthaalldjk.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtywwtienw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hysaishi.cn/gtqquttxzm.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtclfdbkvy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtmgxstkhg.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtchpcgpgk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtajokvyyj.html

[Q83] 大小写转换
来源：http://hz.sysykeji.top/gtypqzdcwv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtbqojlvqa.html

[Q84] 去除首尾空格
来源：http://hz.zhengqikj.top/gtrbapxcuu.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtcewconvc.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtvzivpwsz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shuidangran.top/gtumfbozhv.html

[Q86] 读取 JSON 字段
来源：http://hz.gotoacloud.top/gtmhukeffs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtskusxhbp.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtoxccgjaf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangshuangyany.cn/gtrgjwthzg.html

[Q88] 行转列（条件聚合）
来源：http://hz.xziqi.cn/gtvcqqmzwn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jyoumei.cn/gtejjqpweu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtcovqjtzt.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtiurayxhm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinyuanbaomall.cn/gtthwlutpq.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtkdevgjax.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtdrsezycw.html

================================================================================
来源：http://hz.hfpthk.cn/gtvokhcgyk.html

R. Bash 专题
来源：http://hz.yongpay.top/gtdikmcugm.html

================================================================================
来源：http://hz.redwolf501.top/gtvjbjleja.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gttpspegiu.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtoqycortz.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gtvmqvfuye.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtjyrpqoxk.html

name="Tom"; echo "$name"
来源：http://hz.nwbrower.top/gtcjohbonb.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtnqzlwhjp.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gtsbpfkivt.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gtvxotgmqn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ivvv.top/gtohcyrseo.html

[R05] 参数默认值
来源：http://hz.9152youxi.cn/gtpjavhxsv.html

name="${1:-default}"
来源：http://hz.yj20258.top/gteincxwjc.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtuwkbdzle.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtfyqklcgc.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gthyjmrkmb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cdnleiting.top/gtolddfaik.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtgwzpxcwl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtxnorblbi.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtidbdmmxz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtkmvxdxmd.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtokzlndgy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shzxlz.cn/gtxodfrqgm.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtezjajdyo.html

case "$1" in
来源：http://hz.ehwqpu.com/gtqkwxzill.html

start) echo "启动" ;;
来源：http://hz.tianlin.xyz/gtlaoqrjns.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gthcqxhlof.html

*)     echo "未知命令" ;;
来源：http://hz.hfpthk.cn/gtuxugojlc.html

esac
来源：http://hz.gotoacloud.top/gtfdglirlx.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtnhuikozy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gthchcpeag.html

[R13] for 计数循环
来源：http://hz.c1oappe.top/gtlxpfvpey.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ehwqpu.com/gtbqqfwggv.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtyphsfzdd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtejybwziw.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gtxdwiukim.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtqqfeynst.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtcqpiltnh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtvcsdanhj.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtlpejpcbl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtrwblvcvi.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtreujketc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtrkyvxazn.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtctctztap.html

echo "${#arr[@]}"
来源：http://hz.yj20258888.top/gtewfqzjbv.html

[R20] 关联数组（字典）
来源：http://hz.daxiang520.top/gtrdhfyzhl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gthwkzqzvf.html

[R21] 字符串长度
来源：http://hz.xinyue.icu/gtevcahoea.html

echo "${#s}"
来源：http://hz.birdmap.top/gtawrqlsrz.html

[R22] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtaqoxxhdo.html

echo "${s:0:5}"
来源：http://hz.chenzaomai.com/gtvchvyoiz.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtrtgifczn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtlnrycpum.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtqclpnqqk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtxjxyypbh.html

[R25] 去后缀 / 去前缀
来源：http://hz.dashuyun.cn/gtsogdijec.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gttkrnlota.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtrenpoujb.html

now=$(date +%F); echo "$now"
来源：http://hz.sxryk.cn/gtfuufzhhv.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtmhychznd.html

echo $((1 + 2 * 3))
来源：http://hz.ybcxt.top/gteooswuzt.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtfeextskk.html

echo "scale=2; 10/3" | bc
来源：http://hz.dashuyun.cn/gtlksoxezn.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtceugudxw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtjgbkltoz.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtkippuhwg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.316326.xyz/gtimormfxz.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gtplukzwkm.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtouhdothp.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtpnkbsxwn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigufen.top/gthonzbbeo.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gtpxozpovm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gttirjgulj.html

[R34] 退出时清理
来源：http://hz.kuanghao11.cn/gttvaakguu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtuzthgchy.html

[R35] 后台执行并等待
来源：http://hz.gaohongyu789.top/gtaluwkaft.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.kuanghao11.cn/gtbebsipwx.html

[R36] 并发执行多个任务
来源：http://hz.wangshuangyany.cn/gtdtpfagve.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gtaexnovuz.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gtucepeyvu.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtviiyebkp.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtngvspsgi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zycfv.cn/gttjxkueel.html

[R39] 重定向标准输出与错误
来源：http://hz.cucudq.cn/gthwiodjqr.html

cmd > out.log 2>&1
来源：http://hz.haohaochexian.top/gtpxutaccu.html

[R40] 追加写日志
来源：http://hz.316326.xyz/gtdanbgygt.html

echo "log" >> out.log
来源：http://hz.zhengqikj.top/gtgrxqcgup.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gtxdbalxvt.html

cmd >/dev/null 2>&1
来源：http://hz.kuanghao11.cn/gtvfgggvdx.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtfafgfljr.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtdttzdqnp.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtcpfuphbb.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtmzkvqfti.html

[R44] 按修改时间查找
来源：http://hz.gotoacloud.top/gtxxnaypvk.html

find . -mtime -7 -type f
来源：http://hz.ivvv.top/gtrroaaouf.html

[R45] 批量删除
来源：http://hz.316326.xyz/gtfvuvqcbz.html

find . -name "*.tmp" -delete
来源：http://hz.jiagoushi.top/gtbvhayexq.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gtffciolep.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ivvv.top/gtigdqbjyd.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gthbidkwyh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtvsaksnus.html

[R48] awk 取指定列
来源：http://hz.sxryk.cn/gtrptmfoiy.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuanzx.com/gtiotdrcbd.html

[R49] awk 带条件
来源：http://hz.zhaomingkeji.xyz/gtzsicomut.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtulvoptsa.html

[R50] awk 求和
来源：http://hz.tian-w.cn/gtmxfjojtm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuetiantiany.cn/gtdwqsapcu.html

[R51] 排序去重取前几
来源：http://hz.nwbrower.top/gticppvcuu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtzceanrmc.html

[R52] 统计行数
来源：http://hz.yuanzhike.top/gtpcelcyuq.html

wc -l a.txt
来源：http://hz.bjfxy.top/gtbrnghjqs.html

[R53] 查看文件头与实时尾
来源：http://hz.mhx1999.top/gtkicsmsen.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtibragdra.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gtxowepznb.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gtordqcbze.html

[R55] 压缩与解压
来源：http://hz.jlsjyb.cn/gtzotjgnks.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gzhubu.top/gtcnmjsecr.html

[R56] 远程拷贝
来源：http://hz.hywenlv.cn/gtvfyjeusi.html

scp file user@host:/path/
来源：http://hz.zhixingplan.top/gthlteiutr.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtrxjsfqlt.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtvuwucawu.html

[R58] 下载文件
来源：http://hz.52xcode.cn/gtuwovykwc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtzadhytkc.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtyhwxxqob.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxinkj.top/gttokxuqlq.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtvztgpdqb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xziqi.cn/gttzrzaimy.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtuykftqwz.html

df -h;  du -sh *
来源：http://hz.zhongyouzk.top/gtpukppcye.html

[R62] 找最占空间的文件
来源：http://hz.hfpthk.cn/gtsjzmbdqq.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtwpzqwibn.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtkdbvsvql.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtkjtfvuvs.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtoxzbmwwn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtscootxaz.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtctyybevu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtdofdqcio.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtwxblddxl.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtfdlktmyr.html

[R67] 生成随机十六进制串
来源：http://hz.wangshuangyany.cn/gtipfwplsa.html

openssl rand -hex 16
来源：http://hz.hysaishi.cn/gtujgxkjxi.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gtofjcwlxw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtymzovnln.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtekirlkrz.html

head -c 16 /dev/urandom | base64
来源：http://hz.dianchejie.cn/gtnpiyvjhq.html

[R70] 时间戳与互转
来源：http://hz.guannengcc.top/gtuecglmnn.html

date +%s;  date -d @1700000000
来源：http://hz.tanke756.top/gttpfizxnz.html

[R71] 日期格式化
来源：http://hz.xziqi.cn/gtsttzhmap.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daxiang520.top/gtnamfboro.html

[R72] 等待端口就绪
来源：http://hz.kuanghao11.cn/gtzacxweke.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtkxsjhhyj.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtztvzwavp.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtihynktuq.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gtcczjzavm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhengqikj.top/gtrrapxzme.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtjvdwxmiz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinyuanbaomall.cn/gtaihkzghk.html

[R76] 使用临时文件
来源：http://hz.cashguo.top/gtguoyfpne.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gttxrihgkj.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtkjeoxdij.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtyvszqfbp.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtnryithkh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtqmyizqck.html

[R79] 解析命令行选项
来源：http://hz.cqqwz.cn/gtesuqtumm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gtijwzhery.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtcbgoetbl.html

time ./run.sh
来源：http://hz.xinyue.icu/gtxecoksnc.html

================================================================================
来源：http://hz.shzxlz.cn/gttiwrvnqk.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtfrmluvut.html

================================================================================
来源：http://hz.cqqwz.cn/gtvkmkwoap.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gtvrwbzlom.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtjzinyyed.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhaomingkeji.xyz/gteelgzydg.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gttbupbuve.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj202588.top/gtycpwwlat.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtwjoqflxx.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtldvecqko.html

[S04] C：字符串复制
来源：http://hz.yuxming.cn/gtigxlerke.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtrrixvzpr.html

[S05] C：字符串长度
来源：http://hz.jianghu66.top/gtoglhwggv.html

strlen(s)
来源：http://hz.zhixingplan.top/gtyenwnllr.html

[S06] C：字符串比较
来源：http://hz.xuanzx.com/gteiidovrr.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gteggmmrkc.html

[S07] C：数组遍历求和
来源：http://hz.ivvv.top/gtzcyfbloo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtsldjupsp.html

[S08] C：动态内存分配与释放
来源：http://hz.hywenlv.cn/gtvipdbiei.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtsnynwgml.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtqlakmhks.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.mhx1999.top/gttfydgiyv.html

[S10] C：指针与解引用
来源：http://hz.jqgfzy.top/gtfkrpvydm.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtwxbmmbhy.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtikoqgrzf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ehwqpu.com/gtolzojito.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gtllyiovde.html

fclose(f);
来源：http://hz.quarkkingdee.top/gttwkntgrk.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtxtwrijpe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtiwkxctxo.html

[S13] C：宏定义
来源：http://hz.haohaochexian.top/gtryhahifm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtaoixdzup.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtjeqwnumr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtenowhffm.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtlafnlamf.html

(double) a / b
来源：http://hz.bjfxy.top/gtpoloqase.html

[S16] C：位操作置位
来源：http://hz.redwolf501.top/gttafuhydx.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gttsbffgqu.html

[S17] C：安全拼接字符串
来源：http://hz.ydjk.org.cn/gtgbnthzih.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtxvezfkyd.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtrjruxmrj.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtqmtpmhng.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtyvpxajea.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtjtjxnrnp.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtgdxftcjj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gteeplbmiu.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtddagqmoc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gtedjjppji.html

[S22] C：字符串转数字
来源：http://hz.guowangkeji.top/gtagwdtkce.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtblfscnak.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtqozcxbla.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtfnubqbsr.html

[S24] C：获取本地时间
来源：http://hz.mhx1999.top/gtqlrkzgft.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gttimccsbw.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtpzrvqfaa.html

memcpy(dst, src, n);
来源：http://hz.smart0.xyz/gtujvbimnp.html

[S26] C：内存清零
来源：http://hz.fengsongda.top/gtjhntzepf.html

memset(a, 0, sizeof a);
来源：http://hz.wangdashe.top/gthorwivnd.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtvvquqvoh.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtlwbgjuyk.html

[S28] C：静态变量
来源：http://hz.yueranfly.top/gttpetndsd.html

static int counter = 0;
来源：http://hz.daria6918.cn/gtrozrjsrm.html

[S29] C：变参函数
来源：http://hz.yongpay.top/gtzsmwcwjw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gtqlavdkgx.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtfmaurkbf.html

#ifndef X_H
来源：http://hz.daria6918.cn/gtverwodvy.html

#define X_H
来源：http://hz.hongshengwenyu.top/gtkhiecref.html

#endif
来源：http://hz.wangdashe.top/gtlqbgohgx.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtwezryinz.html

#include <iostream>
来源：http://hz.xuanzx.com/gtjsvdxbim.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtjpzpmdqm.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtqsqwvuwg.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtvgymttvp.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtptxaomux.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pycfn.com/gtipyllmkn.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtgfeosybd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtzqtrswmj.html

[S35] C++：map
来源：http://hz.wangshuangyany.cn/gtytixqkpf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtjavyqjii.html

[S36] C++：unordered_map
来源：http://hz.pycfn.com/gtgzcsfobf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtebtntjxr.html

[S37] C++：set
来源：http://hz.pycfn.com/gtourkrnvm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.andypj.xyz/gthbswwvlx.html

[S38] C++：排序
来源：http://hz.shanyushiyangkeji.top/gtrcbmtnhv.html

std::sort(v.begin(), v.end());
来源：http://hz.chenjidiqi.icu/gttpwzpewu.html

[S39] C++：自定义比较器排序
来源：http://hz.dianchejie.cn/gtptkjykto.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.52xcode.cn/gttjdxxuga.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtrhrcnska.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtngcvryxo.html

[S41] C++：类与构造函数
来源：http://hz.xuanzx.com/gtohhuddya.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gthrcecvwr.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtrpxmifym.html

class B : public Base { public: void f() override {} };
来源：http://hz.zdqjudy.top/gtkqvfvqqj.html

[S43] C++：智能指针
来源：http://hz.kuanghao11.cn/gtpnnpfwvq.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtecqzdyww.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtbpyxclbp.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtgkdcxqpz.html


<!-- 参考信息 -->