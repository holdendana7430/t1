代发 wailian999

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtrgffayal.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtnvfjozsq.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtqixbnsnm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtmabuxspy.html

[Q67] 设置隔离级别
来源：http://hz.hnqzz.top/gtkgwqmzbg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtqhqdqjhd.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gtrfuwnrzj.html

SAVEPOINT sp1;
来源：http://hz.ywan-chungtsiang.top/gtxdcleuyq.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangtech.top/gtzbquvrma.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtossavgfh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gtiryzcgpj.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtqnziokye.html

ANALYZE TABLE users;
来源：http://hz.hnqzz.top/gtervpbcho.html

[Q71] 查看建表语句
来源：http://hz.jinqigfzy.top/gthkbggbnj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydzc1.top/gtallpvyrv.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtcjlppqkp.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtwntrzkka.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtwcehqolk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gtdfsymcuw.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtkehaxtte.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtwjbbtlfa.html

[Q75] 日期格式化
来源：http://hz.feifeiyinyue.top/gtaacwidkw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtxktloftw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daria6918.cn/gtyxyauyjy.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtwrtqowjk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgfzy.top/gtwlejxjco.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gteazmxmqt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sweek.top/gtwwiozknt.html

[Q78] 当前时间
来源：http://hz.vqdsnc.cn/gtxcfeqmxo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gthgtnpant.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtcamshkar.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.9152youxi.cn/gtjdhpwxik.html

[Q80] 字符串截取
来源：http://hz.yj20258888.top/gtoqzynmhm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ehwqpu.com/gtjobculvg.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtzwkxkiif.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinqigfzy.top/gtvfsgzfsi.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtwrwnfilw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ehwqpu.com/gtdwiaiugk.html

[Q83] 大小写转换
来源：http://hz.guannengcc.top/gtpaxcacce.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenzaomai.com/gtixolufhw.html

[Q84] 去除首尾空格
来源：http://hz.birdmap.top/gtgefmqptq.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwnwnocff.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtohpsfkzj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shuidangran.top/gtbegrcpil.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtgbyplttp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gtvmjfeddt.html

[Q87] JSON 字段做条件
来源：http://hz.chenjidiqi.icu/gtuzqtzpxx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ivvv.top/gtgdkovmdk.html

[Q88] 行转列（条件聚合）
来源：http://hz.feifeiyinyue.top/gtyeztzmfh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hammf.cn/gtkgmddlri.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtctevdeki.html

[Q89] 判断表是否存在
来源：http://hz.tianlin.xyz/gtraoalgxq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtdfhmjmjr.html

[Q90] 生成序号列
来源：http://hz.tanke756.top/gtlwkjnrjn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtknwenkoq.html

================================================================================
来源：http://hz.tanke756.top/gtkauiswht.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtzgxhhedp.html

================================================================================
来源：http://hz.ivvv.top/gtiabyxyki.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtatyiztbn.html

#!/usr/bin/env bash
来源：http://hz.jianghu66.top/gtabqqnvmm.html

set -euo pipefail
来源：http://hz.hfpthk.cn/gtrnfipgif.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gtxoxoccsj.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtmcymikra.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtzmbxnpnh.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtpqpyxtdz.html

[R04] 位置参数
来源：http://hz.yvedp.cn/gtdemimdiu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtnviyraje.html

[R05] 参数默认值
来源：http://hz.iojbl.cn/gtivgjiyru.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtrymfdscf.html

[R06] 判断命令是否存在
来源：http://hz.nanxinkj.top/gtihpakjkd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuanzhike.top/gtvvnxfhit.html

[R07] if 判断文件
来源：http://hz.zhongyouzk.top/gtbsyvwicf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtiyeazkob.html

[R08] 数值比较
来源：http://hz.yangfankeji.com/gtthyjdoqs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtmmjltibj.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtqleeavzf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtqaggwoae.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gtyuackstp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.feifeiyinyue.top/gtvjabkupq.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtosrytpgo.html

case "$1" in
来源：http://hz.gzhubu.top/gtflmglxkv.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gtxildiaab.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gtszydphvo.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtlmtqcdld.html

esac
来源：http://hz.xuetiantiany.cn/gtghepzdsk.html

[R12] for 遍历文件
来源：http://hz.zhongyouzk.top/gtabphhqbh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hfpthk.cn/gteiuepwjq.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtxawlbixc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtsydniluu.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gtcykplpjm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtqaxdmgeo.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtszlnsjil.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtlimphhva.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtimvidrdr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtrymjjjax.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gtgnotncgn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gtxbtdmwnv.html

[R18] 遍历数组
来源：http://hz.xingfuxueyuan.xyz/gtkdlxkfyo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.bjfxy.top/gtxulhbkbi.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtllosdpoi.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtemnfrrnt.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtvhxazezw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yueranfly.top/gtneipmzcz.html

[R21] 字符串长度
来源：http://hz.zhiwuduotai.top/gtoqsoakaq.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtdmzqxcjz.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtgugypzti.html

echo "${s:0:5}"
来源：http://hz.dashuyun.cn/gtqwmjturw.html

[R23] 字符串替换
来源：http://hz.jqgufenzy.top/gtkpofcftb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtzdycampf.html

[R24] 大小写转换
来源：http://hz.zhengqikj.top/gtkaunghnr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aibaodan.cn/gtnaybiecf.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtemolanjg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtkpseqcxn.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtqwxrhpio.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtfrgvbjgo.html

[R27] 算术展开
来源：http://hz.ydzc1.top/gtdasmcbcl.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gthkfrstbx.html

[R28] 浮点运算
来源：http://hz.yj20258.top/gttpwpmqdv.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtffatbvxh.html

[R29] 定义函数
来源：http://hz.mhx1999.top/gtmlwvjfqf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gtlgdjvmtw.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtsyxvcobe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.9152youxi.cn/gthoospbhz.html

[R31] 局部变量
来源：http://hz.sweek.top/gthpuwdeoo.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtbkpkvfyu.html

[R32] 参数个数校验
来源：http://hz.cqqwz.cn/gtbumpfqfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sxryk.cn/gtzbtcehbf.html

[R33] 捕获错误并提示行号
来源：http://hz.hnxiangtu.top/gtvcwrhqvg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jianghu66.top/gtfauuaywu.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gtieksjrko.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtsbldjsff.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gttqlipgay.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtlvdnjvlz.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtojgnavgt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtjxwkmkcj.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtxxwcsnpy.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtrnfxznif.html

[R38] 管道串联
来源：http://hz.mhx1999.top/gtcyuxkzsi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj202588.top/gthzdajpvq.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtigknbevk.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtcoasqqtt.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtvicfgxsq.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtzrhjxfux.html

[R41] 丢弃输出
来源：http://hz.jinghuilouyu.cn/gtfdiyrqop.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtzyxmqvco.html

[R42] 输入重定向
来源：http://hz.jinghuilouyu.cn/gtpqwpulzh.html

wc -l < a.txt
来源：http://hz.sysykeji.top/gtwrqkexqw.html

[R43] 按名字查找文件
来源：http://hz.feifeiyinyue.top/gtkxjnmpcs.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gtncsnaigt.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtusnonofj.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gtpqkjmuzj.html

[R45] 批量删除
来源：http://hz.pengpengdd.cyou/gtqycinblr.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gthwvxhnas.html

[R46] 递归替换文件内容
来源：http://hz.jinqigfzy.top/gtudfzoahu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtfugcrgxj.html

[R47] sed 单行替换
来源：http://hz.gogol.net.cn/gtumuspskd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tianlin.xyz/gttppievlx.html

[R48] awk 取指定列
来源：http://hz.vqdsnc.cn/gtevoyilhb.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtsjtpuiee.html

[R49] awk 带条件
来源：http://hz.nanxuanxn.top/gtxxjhermq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtfuldvaxz.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtmovvunar.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtiutwrxco.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtdplslstq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gtipqfbuip.html

[R52] 统计行数
来源：http://hz.meibo888.top/gthnjijacx.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtsdxlvcqd.html

[R53] 查看文件头与实时尾
来源：http://hz.ehwqpu.com/gtxhngieso.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yangfankeji.com/gttrrlmiwx.html

[R54] 比较两个文件
来源：http://hz.jinghuilouyu.cn/gtbrewmggb.html

diff a.txt b.txt
来源：http://hz.hfpthk.cn/gttuibnzyk.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtkwqsaxox.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtugekzlfp.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtkzvmgafl.html

scp file user@host:/path/
来源：http://hz.aizwys.cn/gtxqtmsfzr.html

[R57] 远程执行命令
来源：http://hz.gogol.net.cn/gtgsxhxzda.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtodizgnbx.html

[R58] 下载文件
来源：http://hz.zycfv.cn/gtaxtujicr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtrihqkjey.html

[R59] 发 POST JSON
来源：http://hz.shuidangran.top/gtxkqrulis.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xinyue.icu/gtjuaneqyk.html

[R60] 只看 HTTP 状态码
来源：http://hz.ybcxt.top/gtbjqyiajt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtcoqtgbav.html

[R61] 磁盘占用
来源：http://hz.ywan-chungtsiang.top/gtslmxrxwi.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtjelljnch.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtcvmwnglo.html

du -ah . | sort -rh | head -10
来源：http://hz.zhiwuduotai.top/gtdqjfzffk.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtfztihijs.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtryidztbu.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtvqnwrocl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtjshdgujl.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtqvazuthg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtlpllpxgj.html

[R66] 定时任务
来源：http://hz.cdnleiting.top/gtoxeyxkkq.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtzdsekvft.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigfzy.top/gttpxltvza.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtqqvjjade.html

[R68] 计算文件校验值
来源：http://hz.tianlin.xyz/gtxgpkaxpu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shangyingyoupin.top/gtxxrukcuh.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gtfaycgpeg.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gtvykukody.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtgyytzpud.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gtyxuixiso.html

[R71] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtksjmthkw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtylpiqfbf.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gteqpqsnrm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtmhieisdi.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gtzgmygtst.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gtywpexvtn.html

[R74] 批量重命名
来源：http://hz.xuetiantiany.cn/gttzrkwxvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtrseuxfvj.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gttdphgwxg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.birdmap.top/gtovydkrcu.html

[R76] 使用临时文件
来源：http://hz.c1oappe.top/gtdmpfwlfl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtbjcexsdg.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtwbptgybx.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtlkahzbpn.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtbkcomtaz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sysykeji.top/gtkifztpwd.html

[R79] 解析命令行选项
来源：http://hz.yj20258.top/gtczjajctu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhiwuduotai.top/gtjtoczkvn.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtqixhwout.html

time ./run.sh
来源：http://hz.jianghu66.top/gtpfkosmhu.html

================================================================================
来源：http://hz.yangfankeji.com/gtcjekxzmr.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtftqadkxa.html

================================================================================
来源：http://hz.hammf.cn/gtrtemcrro.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gttcnszpkt.html

#include <stdio.h>
来源：http://hz.quarkkingdee.top/gtygmnmgif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gtguxkyxuz.html

[S02] C：变量与格式化输出
来源：http://hz.sufxvd.cn/gtqyejakey.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtfsdijxoc.html

[S03] C：读入整数
来源：http://hz.daxiang520.top/gtkmhoiqrb.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gthckirydu.html

[S04] C：字符串复制
来源：http://hz.vqdsnc.cn/gtqsjtopzq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.svipenyu.cn/gtyxsqevze.html

[S05] C：字符串长度
来源：http://hz.andypj.xyz/gtgnikoffa.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtkzvxtlub.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gtxlmraqdc.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtmyapashh.html

[S07] C：数组遍历求和
来源：http://hz.hnqzz.top/gttwledmjf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtsdjwzllq.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtubdcudem.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gthdbxronk.html

[S09] C：结构体定义与初始化
来源：http://hz.52xcode.cn/gtjbgotajw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yangfankeji.com/gthgdpidnb.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtrezeyocs.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258888.top/gtojmjiujr.html

[S11] C：逐行读文件
来源：http://hz.zhijiandao.cn/gtvnbxzhbf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtjizzeirr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtftcauhol.html

fclose(f);
来源：http://hz.jqgufenzy.top/gtiaitqqdm.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtmuqzqtbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtdgmqclqj.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtyivgusqu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtwdplxmfi.html

[S14] C：枚举
来源：http://hz.fzhhl.top/gtmspixxdx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtitfonlge.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtnmfclprf.html

(double) a / b
来源：http://hz.svipenyu.cn/gtrdicckpv.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtnamuszvf.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtzqrxpysj.html

[S17] C：安全拼接字符串
来源：http://hz.ydjk.org.cn/gtmiwqxuxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtqyjtfxbf.html

[S18] C：命令行参数
来源：http://hz.gotoacloud.top/gtxtrmhjrp.html

int main(int argc, char **argv)
来源：http://hz.quarkkingdee.top/gtlehrwgzv.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gthmluryrl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtllksmerb.html

[S20] C：二分查找
来源：http://hz.jinyuanbaomall.cn/gtlxmsyzhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gthomlktve.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtyiaojmhy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangtech.top/gtnbfmhimd.html

[S22] C：字符串转数字
来源：http://hz.fengsongda.top/gtuaunidjg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhoulong.xyz/gtdcmhkqvi.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtoclagzta.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yueranfly.top/gtdmuuvhcd.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtgybuhtsf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nwbrower.top/gtxnsdmoae.html

[S25] C：内存拷贝
来源：http://hz.dianchejie.cn/gtluikzrnp.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtlwlitppo.html

[S26] C：内存清零
来源：http://hz.pycfn.com/gtzgqoadsq.html

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gtdhhnqqdy.html

[S27] C：定义常量
来源：http://hz.bjfxy.top/gtcmwwnczt.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtaacrvste.html

[S28] C：静态变量
来源：http://hz.shanyushiyangkeji.top/gtkyiubaip.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtqvtmknlb.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtumaxhdek.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtkirotktb.html

[S30] C：头文件保护
来源：http://hz.shuidangran.top/gtbfexvgwd.html

#ifndef X_H
来源：http://hz.havefunace.top/gtjndasuee.html

#define X_H
来源：http://hz.jlsjyb.cn/gtzrvavwtk.html

#endif
来源：http://hz.tian-w.cn/gtadivztti.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtmydfhjlr.html

#include <iostream>
来源：http://hz.havefunace.top/gtepwwrgqb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtaexljlgd.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gthwxxijxd.html

std::string s = "hi";  s += "!";
来源：http://hz.hongshengwenyu.top/gtabuepueq.html

[S33] C++：vector 增删
来源：http://hz.jyoumei.cn/gtelbivkxl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtawlwzdxe.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtcvdyjcsm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtqcqozoyf.html


<!-- 参考信息 -->