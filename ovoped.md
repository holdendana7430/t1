代发 wailian999

[Q61] 移动平均
来源：http://hz.hywenlv.cn/gtumpmxzdi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhijiandao.cn/gtfptkhcxg.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtcrjfajrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtkpuenect.html

[Q63] 开启事务
来源：http://hz.cdnleiting.top/gtzezqbyaa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangshuangyany.cn/gtrlmcqwyk.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtuwsdkqao.html

COMMIT;
来源：http://hz.sysykeji.top/gtfczelwhy.html

[Q65] 回滚事务
来源：http://hz.c1oappe.top/gtyxkkklic.html

ROLLBACK;
来源：http://hz.fzhhl.top/gturqlvymv.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtquuebbzh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hammf.cn/gtltmbzpwp.html

[Q67] 设置隔离级别
来源：http://hz.jinyuanbaomall.cn/gtohqldlzk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj202588.top/gtjasnmofg.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtwfdgrfxq.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gtgffmwtvt.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtebpgxihk.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtsbejamat.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtlubzarfr.html

[Q70] 更新统计信息
来源：http://hz.hnxiangtu.top/gtikqkiggh.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtabbjqsoo.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtmavsmsgg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gtlgsxesxu.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtumiswvnk.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtgeqsmnok.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtrnvvhwxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gtzjluprrv.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtypoejrkj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sysykeji.top/gtiwzwfkcs.html

[Q75] 日期格式化
来源：http://hz.ppjwa.cn/gtxndzhtwe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtndsrumcj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xinyue.icu/gtvsvervma.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtavultwvu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gtmrlkoktg.html

[Q77] 时间加减
来源：http://hz.jianghu66.top/gtkzzhwhlc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtefsvbnue.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtiqcwupfr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydzc1.top/gtszahbtfr.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gttmcqmdzs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtprcgtqqc.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtkhukcypy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtdugqhldc.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtbnukcjzn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sxryk.cn/gtyrsehocu.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtfrqztsit.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtrjrgprqh.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtxndaqjkr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daria6918.cn/gtdzqmmesr.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gtqpdhndyh.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuanzx.com/gtjzhmwczc.html

[Q85] 数值取整
来源：http://hz.shangyingyoupin.top/gtyifhrlov.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtgvsdudox.html

[Q86] 读取 JSON 字段
来源：http://hz.zycfv.cn/gtntkzbeoy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtvelxaoza.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtqujxtxrd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenzaomai.com/gtymxyndbq.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhixingplan.top/gtvkbpcfve.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtuyprmjpo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtswvdrupj.html

[Q89] 判断表是否存在
来源：http://hz.andypj.xyz/gtfcmbsuox.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtkkdbalki.html

[Q90] 生成序号列
来源：http://hz.hysaishi.cn/gtshopstdr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtrfltpuqw.html

================================================================================
来源：http://hz.yongpay.top/gtvnkvqspm.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gtmrizratd.html

================================================================================
来源：http://hz.redwolf501.top/gtdcrphkqj.html

[R01] shebang 与严格模式
来源：http://hz.c1oappe.top/gtrijuopxj.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtulydozem.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtrzdjnipg.html

[R02] 变量赋值与使用
来源：http://hz.yonumen.top/gtqkvgetge.html

name="Tom"; echo "$name"
来源：http://hz.nanxuanxn.top/gtkzalwknw.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtenrwklgr.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gteslztkhq.html

[R04] 位置参数
来源：http://hz.jlsjyb.cn/gtljcnnafq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtnjjjbtxj.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtchbuzysa.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtpyytdfry.html

[R06] 判断命令是否存在
来源：http://hz.chenjidiqi.icu/gtpngbutbb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtdskiruyp.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gtwoysbzdl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhiwuduotai.top/gtokysywlp.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtzljyrckz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtjhxvvwjy.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtgwglqozq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtarpryyhq.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtkanfdkpg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnqzz.top/gtfjbmbtqi.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtsstwtolu.html

case "$1" in
来源：http://hz.xylfe.cn/gtskveoeiw.html

start) echo "启动" ;;
来源：http://hz.yj202588.top/gtwzkwkogn.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gteztycred.html

*)     echo "未知命令" ;;
来源：http://hz.ydjk.org.cn/gtkqtfbcbq.html

esac
来源：http://hz.jinqigufen.top/gtvioojlwv.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtzqnjuatr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gogol.net.cn/gthokscobn.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtttkchkza.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhiwuduotai.top/gtehpwdurm.html

[R14] C 风格 for
来源：http://hz.chenjidiqi.icu/gteoitqztm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gtypyelmog.html

[R15] while 逐行读文件
来源：http://hz.guannengcc.top/gtqnuadsto.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ppjwa.cn/gtfqvsmvwx.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gtfjkxhhyq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sweek.top/gtwevvecin.html

[R17] 数组定义与取值
来源：http://hz.birdmap.top/gtagbffzyx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtcjuuvbuy.html

[R18] 遍历数组
来源：http://hz.ivvv.top/gtsxmbccly.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtbtjkszvd.html

[R19] 数组长度
来源：http://hz.zhongyouzk.top/gtamcryepz.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtlumahgjy.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtmwbkywvp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fzhhl.top/gtzhgfphsb.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtmdbzknnb.html

echo "${#s}"
来源：http://hz.jyoumei.cn/gtwiecquup.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtuonepyfw.html

echo "${s:0:5}"
来源：http://hz.cdnleiting.top/gtlvkpmenv.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gtsylgbmph.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aizwys.cn/gtcgoumvln.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtheceksvu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gtppnujhqd.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtbqqzbmsw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guowangkeji.top/gtprghingj.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtntjqloql.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gttnqswchi.html

[R27] 算术展开
来源：http://hz.yj20258.top/gtqybfbumu.html

echo $((1 + 2 * 3))
来源：http://hz.zhijiandao.cn/gtfzesardq.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtxlkqtybe.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigufen.top/gtvpcqgoju.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtrwsntlye.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtxfwljuev.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtkublsoel.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gtkqbiyowi.html

[R31] 局部变量
来源：http://hz.zhijiandao.cn/gtdedxcxoq.html

f() { local x=1; echo "$x"; }
来源：http://hz.nwbrower.top/gtmscgpdhr.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtvjbkzihl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtmtjqfhwr.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtcufofxgg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtlkmpncck.html

[R34] 退出时清理
来源：http://hz.shuidangran.top/gtdqhtbjiq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtayammmyl.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gthdugokpv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhixingplan.top/gtyrcxjfnd.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtsumhglwf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gthfqckicc.html

[R37] 把输出赋给变量
来源：http://hz.ydjk.org.cn/gtruseaogl.html

files=$(ls -1)
来源：http://hz.tian-w.cn/gtnthbslzm.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtqacaxwyf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtzwgplbhy.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigufen.top/gtdkflyrms.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtgqjzdgos.html

[R40] 追加写日志
来源：http://hz.yvedp.cn/gtqyumkfyl.html

echo "log" >> out.log
来源：http://hz.cashguo.top/gtyizxeaiu.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtyopsanzw.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtaifeetwd.html

[R42] 输入重定向
来源：http://hz.aizwys.cn/gtuupjvecs.html

wc -l < a.txt
来源：http://hz.nanxinkj.top/gtdydqmazt.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtakskkybm.html

find . -name "*.log" -type f
来源：http://hz.0kj1m.cn/gtexcbdkrz.html

[R44] 按修改时间查找
来源：http://hz.9152youxi.cn/gthycqspeg.html

find . -mtime -7 -type f
来源：http://hz.hnqzz.top/gtgwwiglcd.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtncrumkuv.html

find . -name "*.tmp" -delete
来源：http://hz.feifeiyinyue.top/gtxwbzivrl.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gttmcactbe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhiwuduotai.top/gtlpggiugw.html

[R47] sed 单行替换
来源：http://hz.shangyingyoupin.top/gthkqbdlto.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gtvckrutux.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gtranzdaua.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtcktvoldy.html

[R49] awk 带条件
来源：http://hz.shanyushiyangtech.top/gtgvasytnr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtikyyrqub.html

[R50] awk 求和
来源：http://hz.hywenlv.cn/gtntisfmpk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tianlin.xyz/gtpgibggaz.html

[R51] 排序去重取前几
来源：http://hz.yueranfly.top/gthqpehtxr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gttzpgbumh.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtepjyunuj.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtnnentedx.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtsofefmdj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtjhpqfjjv.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gttmpcogce.html

diff a.txt b.txt
来源：http://hz.jlsjyb.cn/gtbpkepixx.html

[R55] 压缩与解压
来源：http://hz.ppjwa.cn/gtfdykiaox.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hysaishi.cn/gttfyyvyjb.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtscpxawng.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtifbpjfua.html

[R57] 远程执行命令
来源：http://hz.hnxiangtu.top/gtelxqvmkq.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangkeji.top/gtotkoyoxo.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtpztmhsfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtcfqdjtnv.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtojawohmt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nwbrower.top/gteydyxfxr.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtnjmqzcem.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gttxgyzzsd.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtrosjtlka.html

df -h;  du -sh *
来源：http://hz.sysykeji.top/gtqsmsycsc.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtqhlqkcpp.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gthdtzvjwb.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtxbonaqof.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtdegvrudj.html

[R64] 结束进程
来源：http://hz.gogol.net.cn/gtwtalrhaf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gtpjsekftk.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtvrvqsvkk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gtzmefwtjw.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtuffttyvi.html

crontab -e;  crontab -l
来源：http://hz.bjfxy.top/gtihpkpndu.html

[R67] 生成随机十六进制串
来源：http://hz.xziqi.cn/gtfcbztila.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtwxipswrw.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtckwsqwli.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tianlin.xyz/gtvchqvrmm.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gtqeqhsfur.html

head -c 16 /dev/urandom | base64
来源：http://hz.snrcjt.cn/gtjqplsjgc.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtnmathtcc.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtfbhftugc.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtpahyuzsk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.quarkkingdee.top/gtgrpocjkv.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtgjevwhij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtbjxhjghl.html

[R73] 分割大日志
来源：http://hz.nwbrower.top/gtwlpsdvit.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtbditffsw.html

[R74] 批量重命名
来源：http://hz.cdnleiting.top/gtuvxvmkrg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangkeji.top/gtbhlmwwpv.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtziilyrvv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gtpqvytyzj.html

[R76] 使用临时文件
来源：http://hz.haohaochexian.top/gtgblusuxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtfahdmztv.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtcbhwhypm.html

read -rp "请输入: " ans
来源：http://hz.zhoulong.xyz/gtrgyxkdau.html

[R78] 交互式菜单
来源：http://hz.aizwys.cn/gtitogqovc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daria6918.cn/gtsqbcngjr.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtvgixaaat.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtsmejhljn.html

[R80] 查看脚本执行耗时
来源：http://hz.nwbrower.top/gtmwztvtdc.html

time ./run.sh
来源：http://hz.meibo888.top/gtszndnrts.html

================================================================================
来源：http://hz.fzhhl.top/gtunxfnfgc.html

S. C / C++ 专题
来源：http://hz.ywan-chungtsiang.top/gtrgpwznle.html

================================================================================
来源：http://hz.kuanghao11.cn/gtiabkuqas.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtloxujnij.html

#include <stdio.h>
来源：http://hz.jinyuanbaomall.cn/gtrjfcintw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shangyingyoupin.top/gtgornvhau.html

[S02] C：变量与格式化输出
来源：http://hz.ydjk.org.cn/gtkuedhddo.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtyllzcfzp.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtzvvdmjnx.html

int x; scanf("%d", &x);
来源：http://hz.ywan-chungtsiang.top/gtfqrxgbza.html

[S04] C：字符串复制
来源：http://hz.daxiang520.top/gtwspfabfc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.fzhhl.top/gtpdfndnep.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gtuhqahjpm.html

strlen(s)
来源：http://hz.yueranfly.top/gttpmagsbm.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gthohhhqvg.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtudsgooli.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtwaynfedb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.snrcjt.cn/gtsjtjspcq.html

[S08] C：动态内存分配与释放
来源：http://hz.zhaomingkeji.xyz/gtjtbfyvon.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.feifeiyinyue.top/gtqljgyplu.html

[S09] C：结构体定义与初始化
来源：http://hz.daria6918.cn/gtjbklowqu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtoimaohvh.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtxncqbyeh.html

int *p = &a;  *p = 5;
来源：http://hz.ehwqpu.com/gtpugyxccy.html

[S11] C：逐行读文件
来源：http://hz.shzxlz.cn/gtffbzkxnz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xinyue.icu/gtfhepcdls.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtykxezctu.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtajnbemix.html

[S12] C：写文件
来源：http://hz.jqgufenzy.top/gtpaooloux.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtovtauipk.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtazddnxhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gttxctokmw.html

[S14] C：枚举
来源：http://hz.chenzaomai.com/gtnnjicurp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.316326.xyz/gtmtolcymn.html

[S15] C：类型转换
来源：http://hz.snrcjt.cn/gtmpvghdfu.html

(double) a / b
来源：http://hz.yueranfly.top/gtrqofivtp.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtxjllnvlz.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtyiyunbhr.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtuxxmhbjd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuanzhike.top/gtgaaspiaq.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtxfieiyis.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtabhrwrqj.html

[S19] C：快速排序
来源：http://hz.ywan-chungtsiang.top/gtbcmejymn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtuoxutvmv.html

[S20] C：二分查找
来源：http://hz.yj20258.top/gtvinkrorg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtpmqvlxmq.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gttxojreeq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtrwjgnzmv.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtubnroqsn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtedutwnki.html

[S23] C：随机数
来源：http://hz.yongpay.top/gtpmhtnrrx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gtrgaemser.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtgflzabxh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtdkrobijz.html

[S25] C：内存拷贝
来源：http://hz.fengsongda.top/gtkpzvaauy.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtoallgroy.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtvhaotmzc.html

memset(a, 0, sizeof a);
来源：http://hz.yangfankeji.com/gtyizucyew.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gtujlckxqv.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gttpfsxrkx.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gtytkhinil.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtcnqijonn.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtbjsfcrkd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.vqdsnc.cn/gtnxjcbxyb.html

[S30] C：头文件保护
来源：http://hz.zhongyouzk.top/gtbxmagwsl.html

#ifndef X_H
来源：http://hz.snrcjt.cn/gtnkzsoltb.html

#define X_H
来源：http://hz.yj202588.top/gtmmpprlvc.html

#endif
来源：http://hz.c1oappe.top/gttrpprkds.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangtech.top/gtmelwvjdd.html


<!-- 参考信息 -->