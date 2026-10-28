代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daria6918.cn/gtwcgyftos.html

[Q52] 删除指定行
来源：http://hz.snrcjt.cn/gtnmptlvyc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtpldtngpg.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtfvqudhgs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtjrydjxvq.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtrszpzmjp.html

TRUNCATE TABLE logs;
来源：http://hz.yuxming.cn/gtspvqyvmf.html

[Q55] 排名（并列占位）
来源：http://hz.kuanghao11.cn/gtojupgydp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtpfthfdzf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ivvv.top/gtiwtpivnh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtepvhcjbz.html

[Q57] 行号
来源：http://hz.nanxuanxn.top/gtxnftnvmz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.9152youxi.cn/gtgblfjwqy.html

[Q58] 累计求和
来源：http://hz.shanyushiyangkeji.top/gtfatcfzkm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jiagoushi.top/gtyqyrgfep.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtxfndldhy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtecpvsjnh.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtjtcenyhz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gtnqrzpnhr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtgczqfite.html

[Q61] 移动平均
来源：http://hz.shanyushiyangtech.top/gtjzuifdgx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gtphqxdunw.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtfimxqpwo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtgpmseplb.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gtcmfirkkn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shuidangran.top/gtjdexyuaa.html

[Q64] 提交事务
来源：http://hz.birdmap.top/gtxuncpnqt.html

COMMIT;
来源：http://hz.shanyushiyangtech.top/gtszxorpqk.html

[Q65] 回滚事务
来源：http://hz.xylfe.cn/gtyvqzjwrz.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtywqesbcs.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtgskmgbut.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtutrnypzo.html

[Q67] 设置隔离级别
来源：http://hz.zhiwuduotai.top/gtcrkzoyac.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tian-w.cn/gtxsfhqyjj.html

[Q68] 保存点
来源：http://hz.yj20258888.top/gttyrsoyrn.html

SAVEPOINT sp1;
来源：http://hz.jinghuilouyu.cn/gtfpmjzxkp.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtbawlcafw.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtlzoaqmly.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtizkkucrr.html

[Q70] 更新统计信息
来源：http://hz.316326.xyz/gtthlyvslc.html

ANALYZE TABLE users;
来源：http://hz.daxiang520.top/gtngmhqjpz.html

[Q71] 查看建表语句
来源：http://hz.chenzaomai.com/gtqsnitarr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fengsongda.top/gtncixfxcf.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gtgeuxunwl.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtmupcjjip.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gttvninlly.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtvkheakkj.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtkrwczqhx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hfpthk.cn/gterpnxxug.html

[Q75] 日期格式化
来源：http://hz.ydzc1.top/gtyjmtreot.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ppjwa.cn/gtgfkxunef.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtwrkwzfij.html

[Q76] 按天统计
来源：http://hz.quarkkingdee.top/gttbhsvybj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jyoumei.cn/gttmynvmts.html

[Q77] 时间加减
来源：http://hz.316326.xyz/gtiskowqgg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xingfuxueyuan.xyz/gtzpatdeuu.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtzbtnyeye.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cucudq.cn/gtbsjfqacx.html

[Q79] 字符串拼接
来源：http://hz.fzhhl.top/gtehjhhhrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtxcpbcydi.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gttonyanlf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtfcetvhbp.html

[Q81] 字符串替换
来源：http://hz.jyoumei.cn/gtrexoxjwz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pengpengdd.cyou/gtqaukmclh.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtyipvirhg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtgprmvxvy.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gtnkwgxedw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtvcpnmxkv.html

[Q84] 去除首尾空格
来源：http://hz.tanke756.top/gtfkpodsgv.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhoulong.xyz/gtabmqfhtm.html

[Q85] 数值取整
来源：http://hz.yvedp.cn/gtitojkbbq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtowomcbuk.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtkrbuttsy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtqqwqurvl.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtbdhnupdx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtmqufnxra.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtxwmbxqgv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pycfn.com/gtnsxhjvyj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gthetsxpbd.html

[Q89] 判断表是否存在
来源：http://hz.quarkkingdee.top/gttrkykoxs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtqxejbnkg.html

[Q90] 生成序号列
来源：http://hz.cucudq.cn/gtshcxfzwe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtbzqzvssr.html

================================================================================
来源：http://hz.iojbl.cn/gtasneooal.html

R. Bash 专题
来源：http://hz.zhongyouzk.top/gtoamnftnm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtomfqdoiz.html

[R01] shebang 与严格模式
来源：http://hz.zhaomingkeji.xyz/gtscqcapkf.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtcuuyjhic.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtargcxigv.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtfwavgqat.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtkunagdgm.html

[R03] 只读变量
来源：http://hz.9152youxi.cn/gthtraatac.html

readonly PI=3.14
来源：http://hz.gotoacloud.top/gtqeopeomy.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtqohfgbyq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtoejwwkfc.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtxjvjlnma.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtafjffsny.html

[R06] 判断命令是否存在
来源：http://hz.gogol.net.cn/gtxitytmyb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhiwuduotai.top/gthoadyfio.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtcozbedyb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tianlin.xyz/gtkeivnjqb.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtarmatkre.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtvayurgim.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtzifdpjon.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gtccdaimtg.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gttxwizpsw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtfscpkpkb.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gthivzbqfc.html

case "$1" in
来源：http://hz.quarkkingdee.top/gtxkccnwoq.html

start) echo "启动" ;;
来源：http://hz.jqgfzy.top/gtauheyqgy.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtgvwcidrx.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtlevffayj.html

esac
来源：http://hz.nanxinkj.top/gtcuxkzygh.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtcefukysq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jlsjyb.cn/gtktcaprme.html

[R13] for 计数循环
来源：http://hz.zhongyouzk.top/gtzqcvmzqw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtzcamtgxp.html

[R14] C 风格 for
来源：http://hz.sxryk.cn/gtiwxdvrbl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtfbbopuiu.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtcamoduam.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtzetjkypf.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtvofrrlac.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gthfufoxqe.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtcmoatddv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtuwrrbrpx.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtuleswtwz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtwyjbecpd.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtkdissxxc.html

echo "${#arr[@]}"
来源：http://hz.guowangkeji.top/gtlwonaikp.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtahmfmteg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fengsongda.top/gtanroqxpl.html

[R21] 字符串长度
来源：http://hz.birdmap.top/gtbrtpyssr.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtjvfoaxde.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtseeburja.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtekpqxsxp.html

[R23] 字符串替换
来源：http://hz.cdnleiting.top/gtgargzbry.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhongyouzk.top/gtqlmwosya.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtllzxtmpr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtoiyduqss.html

[R25] 去后缀 / 去前缀
来源：http://hz.cqqwz.cn/gtzdwjwybd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.feifeiyinyue.top/gtzujolgye.html

[R26] 命令替换
来源：http://hz.xinyue.icu/gtscxqcwxh.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258888.top/gtbsnlnbyt.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtbexbdgcm.html

echo $((1 + 2 * 3))
来源：http://hz.jinqigufen.top/gtnawpkhvb.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtcykvaqwd.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydzc1.top/gthihfqsiz.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtpjfypesl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gttvwwuvka.html

[R30] 函数返回状态码
来源：http://hz.jinyuanbaomall.cn/gtymzwiili.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinyuanbaomall.cn/gthtuxqlhc.html

[R31] 局部变量
来源：http://hz.zycfv.cn/gtdwthhpfs.html

f() { local x=1; echo "$x"; }
来源：http://hz.guannengcc.top/gtlptibxfj.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtgbenpgxo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtvjqgvsci.html

[R33] 捕获错误并提示行号
来源：http://hz.zhiwuduotai.top/gtrjwjowko.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtygkcgxya.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gthgorzwof.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtsdlelhnq.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gthjukpysn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gtcbdzzukx.html

[R36] 并发执行多个任务
来源：http://hz.9152youxi.cn/gtiaurwpgs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gttchvxsvp.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtnevghmzd.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtgbypyiry.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtcteowddc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gtmvrytunl.html

[R39] 重定向标准输出与错误
来源：http://hz.c1oappe.top/gtvtivsulx.html

cmd > out.log 2>&1
来源：http://hz.daria6918.cn/gtrhwhgnrs.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtcexqttfz.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtjwfoackf.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gtylsedcks.html

cmd >/dev/null 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtfligywgy.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtfuimqder.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtyrocofpd.html

[R43] 按名字查找文件
来源：http://hz.daria6918.cn/gtfepecaxp.html

find . -name "*.log" -type f
来源：http://hz.52xcode.cn/gteogamhuh.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtcubfgvki.html

find . -mtime -7 -type f
来源：http://hz.dashuyun.cn/gtindamwte.html

[R45] 批量删除
来源：http://hz.jqgfzy.top/gtlwkvsesu.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gtlewqslny.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtnkxcvdba.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtqdblnjzw.html

[R47] sed 单行替换
来源：http://hz.cucudq.cn/gtfbleouzr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cqqwz.cn/gtyecqdzly.html

[R48] awk 取指定列
来源：http://hz.ppjwa.cn/gtruqxwdon.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtoeacfnrs.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtchmioukh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtwugvbutf.html

[R50] awk 求和
来源：http://hz.guannengcc.top/gtmkxidorf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtdtgoreub.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtxeyrfsof.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtrfmyawcv.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtqgegfjcw.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtzzyyrgkk.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtqtggaiwt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhongyouzk.top/gtndetqmcd.html

[R54] 比较两个文件
来源：http://hz.ybcxt.top/gtluxsfyod.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtywjnzdpw.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtprhdwlly.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pycfn.com/gtqvvaogyq.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtrewveaak.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtwywzhmnw.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtovmsinhr.html

ssh user@host 'uptime'
来源：http://hz.zhijiandao.cn/gtcflxjcww.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gthsswdsrb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gttsakblpb.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtacjcujkm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtnmshtdwc.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtdotqogft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hysaishi.cn/gtdwgzxxxl.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gthedmenld.html

df -h;  du -sh *
来源：http://hz.meibo888.top/gthdqobnoo.html

[R62] 找最占空间的文件
来源：http://hz.yangfankeji.com/gtsfcduhri.html

du -ah . | sort -rh | head -10
来源：http://hz.xinyue.icu/gtoqaqdths.html

[R63] 内存与进程
来源：http://hz.sysykeji.top/gttbstcawt.html

free -h;  ps aux | grep nginx
来源：http://hz.yuanzhike.top/gtlyofdduh.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtdcijbfnl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangtech.top/gtseypgene.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gthrsswyfk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gtppklbdpm.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtogvjmqgz.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtqnbydrbo.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtddozciuj.html

openssl rand -hex 16
来源：http://hz.tanke756.top/gtevntcssi.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gturuaofwa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuetiantiany.cn/gtirqrzuva.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtwrqmuxhg.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gttivfxidc.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtsriqqppz.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtsqmsthxf.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtgusukgzc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtocpghypk.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtyyvfjgrk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtmsvjauep.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtvhqghdev.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtmlqzvbvy.html

[R74] 批量重命名
来源：http://hz.yonumen.top/gtwtczyehj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gthfcjqjta.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtemnszyho.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtsuhiscpo.html

[R76] 使用临时文件
来源：http://hz.smart0.xyz/gterqulide.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtsrbqnrlb.html

[R77] 读取用户输入
来源：http://hz.jyoumei.cn/gtrlyrfked.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtbkjjfqev.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtbxpeegdm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gteyblzmiv.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtkxdirzsl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtlrlzwzso.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gtpdqtmuun.html

time ./run.sh
来源：http://hz.chenlongwang.top/gtumtdvmjl.html

================================================================================
来源：http://hz.sweek.top/gtzrqnpaqn.html

S. C / C++ 专题
来源：http://hz.dianchejie.cn/gtjynyubup.html

================================================================================
来源：http://hz.zdqjudy.top/gtojrfapsy.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtrlessjbb.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtvgzfqbrm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shzxlz.cn/gtdstmklct.html

[S02] C：变量与格式化输出
来源：http://hz.jinyuanbaomall.cn/gtktzxqjln.html

int a = 10; printf("%d\n", a);
来源：http://hz.zycfv.cn/gtojbntoyz.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtlasznfud.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtpoopuwfp.html

[S04] C：字符串复制
来源：http://hz.xingfuxueyuan.xyz/gtrzktqhxl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cashguo.top/gteubelvcw.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gttmisgadk.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtjgezpfmj.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtudhwicsm.html

strcmp(a, b) == 0
来源：http://hz.wangdashe.top/gtrgskbasq.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtylnonznx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtrmucflwl.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtyaxrsepc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtzyupzvfm.html

[S09] C：结构体定义与初始化
来源：http://hz.xziqi.cn/gtlrnjniam.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangtech.top/gtnklivzjm.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtdcpsshxg.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtpxclrlrp.html

[S11] C：逐行读文件
来源：http://hz.jianghu66.top/gtafbgtido.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtgesxxfai.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtftohcczd.html

fclose(f);
来源：http://hz.shzxlz.cn/gtangbvxja.html

[S12] C：写文件
来源：http://hz.ppjwa.cn/gtulsyjzmh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtmdjmdmqf.html

[S13] C：宏定义
来源：http://hz.aizwys.cn/gtlpmzgqjc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtblfzvbqo.html

[S14] C：枚举
来源：http://hz.pengpengdd.cyou/gtxxoecrlh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtftqnekoo.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtwybmzgum.html

(double) a / b
来源：http://hz.cashguo.top/gtjfczaabn.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gthzwcywdg.html

x |= (1 << 3);
来源：http://hz.hongshengwenyu.top/gtwkmsdjzo.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gthuotxdhi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtabwwlaxw.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtgyhslteb.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtfgxctmnv.html

[S19] C：快速排序
来源：http://hz.shzxlz.cn/gtbdrwpvrp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtbbawlpel.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtwxqkpkwv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtjmqbifpc.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtkjsircuy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtponbeirp.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtqfkvjpnd.html


<!-- 参考信息 -->