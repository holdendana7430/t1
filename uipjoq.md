代发 wailian999

[Q61] 移动平均
来源：http://hz.feifeiyinyue.top/gtdmnmvayw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtrjpkadye.html

[Q62] 分组占比
来源：http://hz.aizwys.cn/gtiqooasza.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtobsrqhmx.html

[Q63] 开启事务
来源：http://hz.9152youxi.cn/gtuypyzlnk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.iojbl.cn/gtdealqamh.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gthljgazas.html

COMMIT;
来源：http://hz.aibaodan.cn/gtqpxcetad.html

[Q65] 回滚事务
来源：http://hz.mhx1999.top/gthntbuxlh.html

ROLLBACK;
来源：http://hz.birdmap.top/gtuprntzyv.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtietxchvy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhijiandao.cn/gtnuoeurlr.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtqvvgnnaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ehwqpu.com/gtttopcqxl.html

[Q68] 保存点
来源：http://hz.cucudq.cn/gtgdfnqhlg.html

SAVEPOINT sp1;
来源：http://hz.316326.xyz/gtzhbxucjo.html

ROLLBACK TO sp1;
来源：http://hz.jianghu66.top/gtxyyrdqqz.html

[Q69] 查看执行计划
来源：http://hz.shangyingyoupin.top/gtgcpyqszg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ywan-chungtsiang.top/gtcsxrrwbm.html

[Q70] 更新统计信息
来源：http://hz.xylfe.cn/gtupueziuy.html

ANALYZE TABLE users;
来源：http://hz.gzhubu.top/gtrhxmonkl.html

[Q71] 查看建表语句
来源：http://hz.smart0.xyz/gtwvtqulrt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hysaishi.cn/gtnmytpdwf.html

[Q72] 查看索引
来源：http://hz.jinghuilouyu.cn/gtodnkmzjp.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtttlrigap.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtnmquvusw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinghuilouyu.cn/gtbzqlxtpc.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtknjidwbh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pycfn.com/gtdvzzqprz.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtgbohgbth.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.316326.xyz/gtbdergjmq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtxhdmbcax.html

[Q76] 按天统计
来源：http://hz.jqgfzy.top/gtiaxlxokl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gtafuzuret.html

[Q77] 时间加减
来源：http://hz.hfpthk.cn/gtcshqamsi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cqqwz.cn/gtcitavbqn.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gttmjorcer.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtfduzzhak.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtssvreker.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shzxlz.cn/gtrbmulxam.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtaxvnixkl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xziqi.cn/gtkeoaplbc.html

[Q81] 字符串替换
来源：http://hz.yj20258.top/gtveemjtkp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtmhwoymjg.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gthwwnkwse.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtponakgel.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtyppqxlgl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jianghu66.top/gtwyaoyukw.html

[Q84] 去除首尾空格
来源：http://hz.hywenlv.cn/gtydeeqhnb.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenlongwang.top/gtmyolkrex.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtglsvkobo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxinkj.top/gthtbhziqu.html

[Q86] 读取 JSON 字段
来源：http://hz.bjfxy.top/gtbxuvloac.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gthpnzcdjw.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtefpatmuz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydjk.org.cn/gtxqwesxtd.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinghuilouyu.cn/gthabzcoer.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dianchejie.cn/gthwcvakxx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hammf.cn/gtvqqrfhxs.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gthgzmbcda.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jyoumei.cn/gtoaahqjer.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gtgazlibsi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenjidiqi.icu/gtwcoopnnj.html

================================================================================
来源：http://hz.dashuyun.cn/gtzbawryxz.html

R. Bash 专题
来源：http://hz.ydjk.org.cn/gtvwfdrcbi.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmwpdlifo.html

[R01] shebang 与严格模式
来源：http://hz.daria6918.cn/gtktbugrlr.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtndiisbil.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gttegvnjyy.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gtlnkfijmv.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtdzstrxmr.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtgzkhongf.html

readonly PI=3.14
来源：http://hz.cqqwz.cn/gtlfxkrdhw.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtvhfbcswu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtaulwjpzt.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtpwjbhlur.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtcopffoot.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtyhacvmne.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gtiuenqjsl.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtnoaxodpx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtcqybcvxc.html

[R08] 数值比较
来源：http://hz.gotoacloud.top/gtwwkhyeuc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yangfankeji.com/gtqpvucbup.html

[R09] 字符串比较
来源：http://hz.andypj.xyz/gttbfdormk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gteldnvdgw.html

[R10] 正则匹配
来源：http://hz.cucudq.cn/gthhvyahwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yueranfly.top/gtbtlafxwg.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtrksastft.html

case "$1" in
来源：http://hz.meibo888.top/gtpecmadup.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gtjgcyjoyf.html

stop)  echo "停止" ;;
来源：http://hz.hywenlv.cn/gtemrtthev.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtmpxcxjwp.html

esac
来源：http://hz.daxiang520.top/gthdeibhwc.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtqgntdrpo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtiiyweavm.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtxcbcwbtj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gthctgoqyu.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gtqscosefs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtttpueneh.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtqzksecqs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtwangpfxw.html

[R16] until 等待条件
来源：http://hz.gzhubu.top/gtifcdcebg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtkkvnqyon.html

[R17] 数组定义与取值
来源：http://hz.vqdsnc.cn/gthajlvkxa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pengpengdd.cyou/gtxzugakfk.html

[R18] 遍历数组
来源：http://hz.bjfxy.top/gtxzhbuafr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtpuqqwair.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gtdwihnwiy.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtxgaaukua.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gtinhcfuvf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj202588.top/gtczdjpmjk.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtvnaqhxdq.html

echo "${#s}"
来源：http://hz.iojbl.cn/gtyfbphqky.html

[R22] 截取子串
来源：http://hz.sxryk.cn/gtnrswqcfx.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gttaxvmlqo.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtkcvgftar.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtaiwaghwq.html

[R24] 大小写转换
来源：http://hz.yongpay.top/gtimbrrbas.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtljrkjoih.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtermlcopk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dashuyun.cn/gtbuauyqks.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtqjrhohun.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtwvkmlfoq.html

[R27] 算术展开
来源：http://hz.jianghu66.top/gtzcgftrwj.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtoywcqgyp.html

[R28] 浮点运算
来源：http://hz.xziqi.cn/gttbgxwzgn.html

echo "scale=2; 10/3" | bc
来源：http://hz.vqdsnc.cn/gthuzlqlft.html

[R29] 定义函数
来源：http://hz.fengsongda.top/gttsrpinkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtryoyyzwc.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gthostyzfj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jianghu66.top/gtbyowhape.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtiqmrqhel.html

f() { local x=1; echo "$x"; }
来源：http://hz.redwolf501.top/gthljvrqan.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gthhmozsml.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtxwzcqpqm.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtmsdnqpvd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtpkdsjufm.html

[R34] 退出时清理
来源：http://hz.jlsjyb.cn/gtsdidekjh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtjgqatpka.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtkddogpvl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtnhvmijmy.html

[R36] 并发执行多个任务
来源：http://hz.zhijiandao.cn/gtktwssdsa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtrtooamnu.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtksxyqefz.html

files=$(ls -1)
来源：http://hz.zhixingplan.top/gtrlmuhrif.html

[R38] 管道串联
来源：http://hz.ppjwa.cn/gtqdsjgowv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nwbrower.top/gtbvrmauif.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtftsfozrc.html

cmd > out.log 2>&1
来源：http://hz.jinyuanbaomall.cn/gtvyklbuaf.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtrkfhjlof.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtftanygsn.html

[R41] 丢弃输出
来源：http://hz.fengsongda.top/gtwxwsqrwv.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtdvpvckwr.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtvqictjmw.html

wc -l < a.txt
来源：http://hz.zhijiandao.cn/gtbalvjstb.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtfmqdigrw.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtqvzbjoml.html

[R44] 按修改时间查找
来源：http://hz.mhx1999.top/gtghowvfqp.html

find . -mtime -7 -type f
来源：http://hz.pengpengdd.cyou/gtaasbgqaz.html

[R45] 批量删除
来源：http://hz.guannengcc.top/gtovwqpomk.html

find . -name "*.tmp" -delete
来源：http://hz.52xcode.cn/gtxdeatazm.html

[R46] 递归替换文件内容
来源：http://hz.meibo888.top/gtojyuavux.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtcvrmjkwi.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtmtfoczfa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.havefunace.top/gtpqdmkmdd.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtckcqdmmv.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtsriouajh.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtydxcinws.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhaomingkeji.xyz/gtkfmdhbha.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtcgxjlhif.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtypgsvxyx.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtpgkaggpu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gthterjccg.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gtbqdfqbgk.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtrpvqbyzh.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gtulniyxrq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxuanxn.top/gtksxgqzsj.html

[R54] 比较两个文件
来源：http://hz.tian-w.cn/gtuuchiufy.html

diff a.txt b.txt
来源：http://hz.dianchejie.cn/gtscmhsnhf.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtmtpxgvjz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtazmmmhdn.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtloxuiwku.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gtjblzpaoh.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtivcvprrq.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gttxgwuwby.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gtkshlmpxt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.birdmap.top/gtjsrfyput.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtugmrnjff.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtjxskglep.html

[R60] 只看 HTTP 状态码
来源：http://hz.nwbrower.top/gtnbojdemg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sufxvd.cn/gtxfitwdwh.html

[R61] 磁盘占用
来源：http://hz.gzhubu.top/gtylvvulnu.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtkulklwdk.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtxjbyipeo.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gttpzonrjy.html

[R63] 内存与进程
来源：http://hz.zhixingplan.top/gttdonufuo.html

free -h;  ps aux | grep nginx
来源：http://hz.9152youxi.cn/gtpeyamsxj.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtvelvzviv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtqnrxsawb.html

[R65] 查看端口占用
来源：http://hz.shzxlz.cn/gtzzejboop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtyjajogkl.html

[R66] 定时任务
来源：http://hz.xuanzx.com/gteqzinmkd.html

crontab -e;  crontab -l
来源：http://hz.redwolf501.top/gtwpvtrnrm.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtsoeionxm.html

openssl rand -hex 16
来源：http://hz.meibo888.top/gtkosayiyk.html

[R68] 计算文件校验值
来源：http://hz.cheryme.top/gtkznvwnpy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtgkigzjyl.html

[R69] 生成随机密码
来源：http://hz.svipenyu.cn/gtceyqljqw.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtepklrptg.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gttjfayvwb.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtggkqoazf.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtwupwwctv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtrvawcwex.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gthikgpsrt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtnlndkuyv.html

[R73] 分割大日志
来源：http://hz.tian-w.cn/gtjlsdmtsl.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtefmmfkmv.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtcaccjbbo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guowangkeji.top/gtcewwuead.html

[R75] 导出环境变量
来源：http://hz.sxryk.cn/gthiiuqihs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gteqquxojm.html

[R76] 使用临时文件
来源：http://hz.daria6918.cn/gtbrauwpvf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtvrieekdx.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtkcminyaa.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtefrdezmn.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtjajnqrhv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuxming.cn/gtayharobc.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gtvyehkkgg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xylfe.cn/gtoxogcdga.html

[R80] 查看脚本执行耗时
来源：http://hz.zhixingplan.top/gtyfkkuffm.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtxwuwedny.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvqyopmqb.html

S. C / C++ 专题
来源：http://hz.hfpthk.cn/gtyawumphn.html

================================================================================
来源：http://hz.yonumen.top/gtxceutkev.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtnswiuoln.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtukgkwtoj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daxiang520.top/gtesxqvdwo.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gtnhmkmxox.html

int a = 10; printf("%d\n", a);
来源：http://hz.gotoacloud.top/gtoafmdjtd.html

[S03] C：读入整数
来源：http://hz.shanyushiyangkeji.top/gtumuuhtpz.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtgcpuezyt.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtubtwlfcs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangkeji.top/gtcdwcqmwe.html

[S05] C：字符串长度
来源：http://hz.aizwys.cn/gtjwjmewbx.html

strlen(s)
来源：http://hz.hfpthk.cn/gtixwultxu.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gtirvcbauh.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtavdikuqp.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gttnkhlxxq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gteqbkcqkz.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtvxopbvcx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtvprtpmnw.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtqmxdbvwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gthtgyplax.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gtpzbnzivq.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtibzgfcch.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtoiolgcyv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gthkjsmcth.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtytumfcqi.html

fclose(f);
来源：http://hz.yj202588.top/gtfgotnqkn.html

[S12] C：写文件
来源：http://hz.hnxiangtu.top/gtjjiqssol.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fengsongda.top/gtgbgiirqw.html

[S13] C：宏定义
来源：http://hz.zhoulong.xyz/gtswbtevsg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangkeji.top/gtrhtvpyfj.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gtmbggqsvb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ehwqpu.com/gttpfbddql.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtngksdpwe.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtjrdwuquu.html

[S16] C：位操作置位
来源：http://hz.fzhhl.top/gtedugjowq.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gttswvqiom.html

[S17] C：安全拼接字符串
来源：http://hz.cashguo.top/gtuuyccymq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtamlqpyqb.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtngntlgah.html

int main(int argc, char **argv)
来源：http://hz.xylfe.cn/gtmsyiryni.html

[S19] C：快速排序
来源：http://hz.fzhhl.top/gtpmiyjnzh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtfxaxpnod.html

[S20] C：二分查找
来源：http://hz.xylfe.cn/gtpvdzcsuy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtjmihvwgv.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtcrshazuk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtzqabzdpq.html

[S22] C：字符串转数字
来源：http://hz.yj20258.top/gtefjcfhsh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtzwyercfr.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtsajvolii.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuanzhike.top/gtvdntbapv.html

[S24] C：获取本地时间
来源：http://hz.bjfxy.top/gtgakovtud.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gtjgvbqhpc.html

[S25] C：内存拷贝
来源：http://hz.jinghuilouyu.cn/gtuwmxkyyr.html

memcpy(dst, src, n);
来源：http://hz.zdqjudy.top/gtbvykscse.html

[S26] C：内存清零
来源：http://hz.pycfn.com/gtlobafpas.html

memset(a, 0, sizeof a);
来源：http://hz.daria6918.cn/gtxpxsypnd.html

[S27] C：定义常量
来源：http://hz.shuidangran.top/gtsipetxss.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtaraagyxu.html

[S28] C：静态变量
来源：http://hz.yuanzhike.top/gthjwvbife.html

static int counter = 0;
来源：http://hz.jianghu66.top/gtfskbfybv.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtvnijjcrj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cashguo.top/gttsxoqfmj.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtymaylkih.html

#ifndef X_H
来源：http://hz.pycfn.com/gtcecouvnr.html

#define X_H
来源：http://hz.shuidangran.top/gtvcrtbdmd.html

#endif
来源：http://hz.yongpay.top/gtvpmffust.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gtzzqbelxg.html


<!-- 参考信息 -->