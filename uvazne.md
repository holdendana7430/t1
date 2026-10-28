代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.jlsjyb.cn/gtgyybbkrg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtisgcjntv.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gtkuccbqow.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gttjgwlbkx.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtlwdmrodg.html

[Q69] 查看执行计划
来源：http://hz.nanxuanxn.top/gtbtiknhjp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shuidangran.top/gtnnolzpur.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtvejsxxyn.html

ANALYZE TABLE users;
来源：http://hz.bjfxy.top/gtqgdtcftf.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gtatrmakqm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhixingplan.top/gtnmroobsp.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtwsjrklez.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtstowrtvl.html

[Q73] 查看表状态
来源：http://hz.quarkkingdee.top/gtxrmiaton.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtwachjodk.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtgxbcdbms.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ehwqpu.com/gtzcdadnti.html

[Q75] 日期格式化
来源：http://hz.zhiwuduotai.top/gtjiwubwdz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gttjflwcpr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jiagoushi.top/gtaheutvkz.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtrvibodfs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinyuanbaomall.cn/gttnkekisy.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtcncllyvz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gotoacloud.top/gtfboeyvce.html

[Q78] 当前时间
来源：http://hz.andypj.xyz/gtcvmmwhto.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gthrfaztni.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtumikmbrd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gttyvrykms.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtfkighsdj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtgxykghju.html

[Q81] 字符串替换
来源：http://hz.yueranfly.top/gtidnfpohl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtzhomfpgc.html

[Q82] 字符长度与字节长度
来源：http://hz.pengpengdd.cyou/gtfbuisrel.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtkfumkxrl.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtlhnnadkc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtjstixziz.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtqjmdvgfl.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtfqrwlhhm.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtzjwbktsq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yongpay.top/gtxypicrum.html

[Q86] 读取 JSON 字段
来源：http://hz.yuanzhike.top/gtjzfumvda.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtkesfwzkj.html

[Q87] JSON 字段做条件
来源：http://hz.yanxiufei.cn/gtkxxltsep.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtenhocfut.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtpyfddjaa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gtpsqmpfzd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtacfndvuk.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtpxpltknk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258888.top/gtvornwtio.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtmjmnjxfk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daxiang520.top/gtcgtoyqrl.html

================================================================================
来源：http://hz.gzhubu.top/gtlilqgfpz.html

R. Bash 专题
来源：http://hz.cashguo.top/gtjfvqcizo.html

================================================================================
来源：http://hz.zhixingplan.top/gtoyzgneac.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gtphhtaxhc.html

#!/usr/bin/env bash
来源：http://hz.zhongyouzk.top/gtlwowtzjw.html

set -euo pipefail
来源：http://hz.c1oappe.top/gtjqsrkujp.html

[R02] 变量赋值与使用
来源：http://hz.mhx1999.top/gtkniinybl.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtwpxwtioc.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtugzvbinv.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtldmkwmah.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtfqtbzsvp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gttttryyck.html

[R05] 参数默认值
来源：http://hz.gzhubu.top/gtgpqefmzn.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gtvnodqbwd.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtgpnswlbb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtmvgdmeaf.html

[R07] if 判断文件
来源：http://hz.hnxiangtu.top/gtzrgoueip.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtyukasomp.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtfljiiriw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.316326.xyz/gtisapzrnu.html

[R09] 字符串比较
来源：http://hz.aibaodan.cn/gtsnwkwcks.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cheryme.top/gtxxzjvtwq.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gtdgmckkqg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtvwxgbvxc.html

[R11] case 多分支
来源：http://hz.fengsongda.top/gtcctgumuh.html

case "$1" in
来源：http://hz.yongpay.top/gtyqxxraya.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gtpyjbldto.html

stop)  echo "停止" ;;
来源：http://hz.xziqi.cn/gtcabwpeik.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtvdmubnrw.html

esac
来源：http://hz.shuidangran.top/gtkoumjmgb.html

[R12] for 遍历文件
来源：http://hz.jianghu66.top/gtfhavaxzd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtssiqifdl.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gthiytbjbu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtkqpqfhbg.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtzvqwmlrd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtckykuwpf.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtjjhbqhhf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtimhlwtix.html

[R16] until 等待条件
来源：http://hz.cqqwz.cn/gtstuinijc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jyoumei.cn/gtacyrizfs.html

[R17] 数组定义与取值
来源：http://hz.hysaishi.cn/gtipqupbin.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxinkj.top/gtlfwlasfg.html

[R18] 遍历数组
来源：http://hz.ywan-chungtsiang.top/gtdbsasgfc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinghuilouyu.cn/gtqizoltjy.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gtliojheji.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtnsmqbczh.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtzgecymfv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.0kj1m.cn/gtqjrteery.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtsarltgol.html

echo "${#s}"
来源：http://hz.dashuyun.cn/gtczqzxdok.html

[R22] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtdhurhvpv.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtxrcymhmd.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtujqjgzaa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtmlijxduz.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtefxoqqbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gtexlolbre.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtxqcduxmh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtbpkjrgzy.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gtqjzvbgop.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtukzkwrwo.html

[R27] 算术展开
来源：http://hz.tianlin.xyz/gtehdjddle.html

echo $((1 + 2 * 3))
来源：http://hz.c1oappe.top/gtdjsiegud.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtramgehbm.html

echo "scale=2; 10/3" | bc
来源：http://hz.ybcxt.top/gtytvbftog.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtmvnzgmbp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtmiqjnooo.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtdxrhfuil.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.smart0.xyz/gttdefmxpm.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtjtfelkly.html

f() { local x=1; echo "$x"; }
来源：http://hz.xziqi.cn/gtrczpcbkd.html

[R32] 参数个数校验
来源：http://hz.jyoumei.cn/gtqxntckvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtakuzlpjs.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtiafyiiju.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtulnrlubn.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gthlogkthm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtzzupksee.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gtqpjffpbv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258.top/gtxfdfzspn.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtqdsikukv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gtowjiqtww.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtxupiwuyz.html

files=$(ls -1)
来源：http://hz.yj20258.top/gtaxduruwr.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtdfwdrgzl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jlsjyb.cn/gtpnthjirw.html

[R39] 重定向标准输出与错误
来源：http://hz.0kj1m.cn/gtwqotnslb.html

cmd > out.log 2>&1
来源：http://hz.cqqwz.cn/gtgyhdhfic.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtjvfgjadb.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtzqwouxdl.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtglvotfhv.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtplqaqntu.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtoqczbdkv.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtmcdxhgfy.html

[R43] 按名字查找文件
来源：http://hz.jinqigfzy.top/gtdfljasrs.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtsefsuhde.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtfisfdvah.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtxavrlxok.html

[R45] 批量删除
来源：http://hz.svipenyu.cn/gtwzpxqohh.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gttyyouots.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtlfiedtqo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtzrgfzmdo.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtlucjxqqo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtcgnuinhp.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtwrgcqbmo.html

awk '{print $1, $3}' a.txt
来源：http://hz.ivvv.top/gtefreqsum.html

[R49] awk 带条件
来源：http://hz.gotoacloud.top/gtvsuaubxd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtkycdddhh.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gtfvxaqaed.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gttfgpsrpr.html

[R51] 排序去重取前几
来源：http://hz.iojbl.cn/gtwgawxecu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtmfosmrdp.html

[R52] 统计行数
来源：http://hz.zycfv.cn/gtqyevolik.html

wc -l a.txt
来源：http://hz.cheryme.top/gtojzhdpnc.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtgqevdldi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtnlygdghk.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtsqzohsty.html

diff a.txt b.txt
来源：http://hz.zhaomingkeji.xyz/gtlnnqjhen.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtiqfmjgfz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gtyyeeecjf.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtjhkxzlqo.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gtznupsqrm.html

[R57] 远程执行命令
来源：http://hz.hysaishi.cn/gtltpulceh.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtxirmsmen.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtoijqlejn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sweek.top/gtormwtnif.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtqlfzkfcp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtmzehrgyo.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtphhmsasn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtyrxgaref.html

[R61] 磁盘占用
来源：http://hz.zhoulong.xyz/gtdwpoucky.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtveuyxemb.html

[R62] 找最占空间的文件
来源：http://hz.quarkkingdee.top/gtqeiybkfg.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtekxuqqcc.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtfmppiyjp.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtsrhskstx.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtsbqqtsoc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtcounebjf.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtguwyytqs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gtatmkmstb.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtcvcskiyh.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtyuwglbzg.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gtthdromkf.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtcbpgsfcg.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtburuncsg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gthxppybie.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtdnlgfyku.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtspqvnuxp.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtauiahxgz.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gtqoyzvjjk.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtbcmovcqb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtixpawzce.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gttpwstddr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ppjwa.cn/gtpflfyttn.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtphqryjtz.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtzksukfwq.html

[R74] 批量重命名
来源：http://hz.tanke756.top/gtksrwkark.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cashguo.top/gtujmwyicq.html

[R75] 导出环境变量
来源：http://hz.birdmap.top/gtkaztmnar.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtgfoodxou.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtcgeovxxc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtlyyyyssz.html

[R77] 读取用户输入
来源：http://hz.yongpay.top/gtjepjbudi.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtqzacnvkn.html

[R78] 交互式菜单
来源：http://hz.bjfxy.top/gtthejrqqi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtijyjmgsp.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtjzyfhasn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shangyingyoupin.top/gtwjziygkd.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtacvclafc.html

time ./run.sh
来源：http://hz.ybcxt.top/gtpworkhch.html

================================================================================
来源：http://hz.hnqzz.top/gtuiijsoro.html

S. C / C++ 专题
来源：http://hz.ivvv.top/gtaxyjqlij.html

================================================================================
来源：http://hz.jqgfzy.top/gtlannrpjg.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtbkklnphx.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gtezyqzwpb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtqsscuzag.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtlrsawmbo.html

int a = 10; printf("%d\n", a);
来源：http://hz.svipenyu.cn/gtwtqguixf.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gtbroeuizx.html

int x; scanf("%d", &x);
来源：http://hz.birdmap.top/gtzsaagwtq.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtjxdidjek.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtrsjphqyh.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtqxrmfdcg.html

strlen(s)
来源：http://hz.mhx1999.top/gtoxqafsbm.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtewprkdwx.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtwrvjhbcg.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gtpqzgkqcg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtezeszcoy.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtgbxhecny.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtvqfrurfb.html

[S09] C：结构体定义与初始化
来源：http://hz.ywan-chungtsiang.top/gtfoeipxvs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtpieedlbf.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtoudaqsku.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtalhiytvv.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtdjozmcoc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.vqdsnc.cn/gtnnvulqyq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xylfe.cn/gtdjwdehit.html

fclose(f);
来源：http://hz.xuanzx.com/gtfhcpoiwt.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtvubhbdii.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtiejeozfx.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gthicsqulm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhongyouzk.top/gtgjoihmea.html

[S14] C：枚举
来源：http://hz.jqgfzy.top/gtzfibnydt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuanzhike.top/gtxawycivq.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtpdwtrjlw.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtcajkatlo.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gthkabxqki.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtwrnnlnbk.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtogdfzhus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtleywvbnl.html

[S18] C：命令行参数
来源：http://hz.nanxuanxn.top/gtodfuocaf.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangkeji.top/gtyiwslmbz.html

[S19] C：快速排序
来源：http://hz.pengpengdd.cyou/gtqrtwqsxw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtvvhavewm.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtkylqmggn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtvjsylocw.html

[S21] C：字符类别判断
来源：http://hz.yj202588.top/gtbnwuixlj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtiugafcow.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtubihhxfg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtjeqtbyqz.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtfqtsynqn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shangyingyoupin.top/gtzwtwrxhk.html

[S24] C：获取本地时间
来源：http://hz.hysaishi.cn/gtvfpdamdy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtwhkiagdz.html

[S25] C：内存拷贝
来源：http://hz.hysaishi.cn/gtwpetknmj.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gthvzicwwn.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gtmseuqevs.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtkbucloda.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtdzwyoxub.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gteyexztkz.html

[S28] C：静态变量
来源：http://hz.yj202588.top/gtghydrxcb.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtxftvzdmz.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtunxtfpiq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtzepastte.html

[S30] C：头文件保护
来源：http://hz.feifeiyinyue.top/gtwepzzqpv.html

#ifndef X_H
来源：http://hz.cqqwz.cn/gtwiadvkld.html

#define X_H
来源：http://hz.guowangkeji.top/gttbuzwcql.html

#endif
来源：http://hz.yueranfly.top/gtjrbgjrie.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtrxlgpxdt.html

#include <iostream>
来源：http://hz.jqgfzy.top/gtoakzywqs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgfzy.top/gttylgbfvs.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtxfosfwsr.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gtdfhkklyb.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtgixbmkyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ppjwa.cn/gtdqxkkwuu.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtxvzhlfjh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhiwuduotai.top/gtxesyxoiq.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtikrybfix.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtntsjlkxc.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtbhqwozrp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtmhqmwiqy.html


<!-- 参考信息 -->