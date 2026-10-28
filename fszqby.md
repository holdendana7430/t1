代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtkkfjagzs.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gtauareqjp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtbvcqsuix.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gtfdxenqdo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.9152youxi.cn/gtzzvmzljf.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtkrqkyaob.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtqxkcmwtk.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtrponhtcj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtzodgmqut.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtffrnvrns.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gttgrlneft.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtrmozsvvo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuanzx.com/gtzyijqbgy.html

[Q58] 累计求和
来源：http://hz.sysykeji.top/gtxeyrfgho.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fzhhl.top/gtezrmynho.html

[Q59] 分组内累计
来源：http://hz.zycfv.cn/gthjhhxlvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jyoumei.cn/gtpwpqtfdz.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtjorcqifo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangtech.top/gtbzyglerf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtylyrkosn.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtpheyfgha.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtmqsepopg.html

[Q62] 分组占比
来源：http://hz.yj202588.top/gthabzlubp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtptxpkevm.html

[Q63] 开启事务
来源：http://hz.fzhhl.top/gtwzoxuezi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.316326.xyz/gtedkceyut.html

[Q64] 提交事务
来源：http://hz.shuidangran.top/gtqxismovj.html

COMMIT;
来源：http://hz.fzhhl.top/gtgvdikpad.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtecjsdjrj.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtwitzjmpz.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtdbmndtoz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnqzz.top/gthgvcacyl.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtkrwpivzb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtklflhgpd.html

[Q68] 保存点
来源：http://hz.gzhubu.top/gtsskjqqax.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtagwkqsth.html

ROLLBACK TO sp1;
来源：http://hz.daxiang520.top/gtzhdkqytf.html

[Q69] 查看执行计划
来源：http://hz.c1oappe.top/gtggkjeakj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258.top/gtdmwvlyml.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtkddowbzu.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtjpxfhwty.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gtxsambtvb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtzfddudzt.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gttemxkink.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtcwdivgrj.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gtbckqmmqr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gtlrnjcozl.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gttwwwlddu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gtgtazsvuh.html

[Q75] 日期格式化
来源：http://hz.iojbl.cn/gtorlgqwuk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtebkndqmm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhiwuduotai.top/gtjyvaldyc.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtrqhtizdb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yvedp.cn/gtwyidpenr.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gttyuqnhad.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtqabpzrhy.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtrpuvworm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gtkdzwfqsp.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtlbbgrigx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtdqkrnktk.html

[Q80] 字符串截取
来源：http://hz.gzhubu.top/gtummtsyiq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxuanxn.top/gtfnykcuie.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtghimhtam.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtbjxhsbqm.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtjglanvul.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.haohaochexian.top/gtgpfqsppj.html

[Q83] 大小写转换
来源：http://hz.yvedp.cn/gtyyeunodj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtfhcnyhtx.html

[Q84] 去除首尾空格
来源：http://hz.quarkkingdee.top/gtwvypbbvu.html

SELECT TRIM(name) FROM users;
来源：http://hz.pycfn.com/gtbtcclcfz.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gtwturfowm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtufchbtie.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtcqonofpz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtkddjgqhw.html

[Q87] JSON 字段做条件
来源：http://hz.cashguo.top/gtjahnjmmk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtbjvxfmtv.html

[Q88] 行转列（条件聚合）
来源：http://hz.kuanghao11.cn/gtjukshqlo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangshuangyany.cn/gtmlhnmgdy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangshuangyany.cn/gtwlpaxzff.html

[Q89] 判断表是否存在
来源：http://hz.smart0.xyz/gtdevtyiel.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.c1oappe.top/gtazirbrcv.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtlsynhjvg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xinyue.icu/gtqjesorzh.html

================================================================================
来源：http://hz.yj20258.top/gtwglksxik.html

R. Bash 专题
来源：http://hz.havefunace.top/gtveeiofni.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzdnbppeh.html

[R01] shebang 与严格模式
来源：http://hz.shangyingyoupin.top/gtjkcbmdff.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtpqwswdqg.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gteedaiwws.html

[R02] 变量赋值与使用
来源：http://hz.ydzc1.top/gtbwdmxspl.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtltdatxfy.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtpdmhrejh.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtbjmdxkfr.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtchjbkhnq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtqrmmeqbn.html

[R05] 参数默认值
来源：http://hz.jiagoushi.top/gtlwmhewnz.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gtupdhbpdl.html

[R06] 判断命令是否存在
来源：http://hz.9152youxi.cn/gttqnjfrdt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtboghhyuh.html

[R07] if 判断文件
来源：http://hz.chenlongwang.top/gtnvdtzbgv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtparmqexl.html

[R08] 数值比较
来源：http://hz.jyoumei.cn/gtfhpbhklm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258.top/gtgruxaayt.html

[R09] 字符串比较
来源：http://hz.cheryme.top/gtykgkfbzs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.52xcode.cn/gtxdaxyrhs.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtostcuzsb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aizwys.cn/gtsktagmkx.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtrmykufff.html

case "$1" in
来源：http://hz.wangdashe.top/gtefjejmzm.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtazdhdpdu.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtxxzkuhnd.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gtyomwdrtn.html

esac
来源：http://hz.shuidangran.top/gtrkztvjex.html

[R12] for 遍历文件
来源：http://hz.quarkkingdee.top/gthtiiinvu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnqzz.top/gtsnnstyzh.html

[R13] for 计数循环
来源：http://hz.ybcxt.top/gtlzoibblh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gtgpjwiwgy.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtxxevykpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hysaishi.cn/gtdfjmvohy.html

[R15] while 逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gtebhrgyqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yangfankeji.com/gtdexcolud.html

[R16] until 等待条件
来源：http://hz.yj20258.top/gtzdlaviso.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cdnleiting.top/gtcojwlwvl.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtjmnpxoct.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gteedwlmie.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtkiuybtzc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtnmkdhnfe.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtmskusmvi.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtxodtilic.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtkxjdzlon.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ivvv.top/gtnutqstzu.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtkfvmdjng.html

echo "${#s}"
来源：http://hz.cashguo.top/gtmueyzrpf.html

[R22] 截取子串
来源：http://hz.cashguo.top/gtyqkhffif.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtfutioifp.html

[R23] 字符串替换
来源：http://hz.andypj.xyz/gtkzyryebo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pengpengdd.cyou/gtbewseubf.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtlrebmarb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtnbkacsoa.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtcueeqqjn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxinkj.top/gtqsfbukmq.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtqsofykon.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gthwtgxdok.html

[R27] 算术展开
来源：http://hz.bjfxy.top/gtxjflwxov.html

echo $((1 + 2 * 3))
来源：http://hz.hywenlv.cn/gtkhxxfjgs.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtzqzluiij.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gthjuahczb.html

[R29] 定义函数
来源：http://hz.guannengcc.top/gtjdvhsccn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtasqtreni.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtimojwqgo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gtiaqaaadb.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtabobvswl.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtmmsakkfw.html

[R32] 参数个数校验
来源：http://hz.gaohongyu789.top/gtxdvkqwfi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.pycfn.com/gttludezzh.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtopjeloxp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtymbzmltt.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtzlrbjzez.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gtqaqkyelu.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gtmyjmtwke.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtxrefyzow.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtrbrwvpvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gtqgslynng.html

[R37] 把输出赋给变量
来源：http://hz.svipenyu.cn/gtptejujby.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtfqfgyreb.html

[R38] 管道串联
来源：http://hz.cashguo.top/gtjiivfjvb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtikrbqaki.html

[R39] 重定向标准输出与错误
来源：http://hz.aizwys.cn/gtylvcfuoj.html

cmd > out.log 2>&1
来源：http://hz.dashuyun.cn/gtnwojhbrd.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gtfmiqrezc.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtuzqobddc.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtkcrxbgre.html

cmd >/dev/null 2>&1
来源：http://hz.pengpengdd.cyou/gtgoniytcm.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtvpkylpol.html

wc -l < a.txt
来源：http://hz.jinyuanbaomall.cn/gtxkzncotq.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gtjsveqbzw.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtblijfmud.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gtfbolcldv.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gttltxxkju.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtdyswatfu.html

find . -name "*.tmp" -delete
来源：http://hz.0kj1m.cn/gtplrugmfn.html

[R46] 递归替换文件内容
来源：http://hz.jianghu66.top/gtomwdovdw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj202588.top/gtznnucteb.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gtlcnugmxv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.redwolf501.top/gtlhvfineh.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtxrdkotzp.html

awk '{print $1, $3}' a.txt
来源：http://hz.haohaochexian.top/gtekcyallb.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtiwojehrq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.haohaochexian.top/gtzyzauodp.html

[R50] awk 求和
来源：http://hz.fzhhl.top/gtndlpdkpm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtfzkasgjb.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gtfopziqyu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangshuangyany.cn/gttbdwzait.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtxgedqfkb.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtlvqdbrfe.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtxcvpwpoi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gtztfrtqcb.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtxoawzpsi.html

diff a.txt b.txt
来源：http://hz.yueranfly.top/gtzwazmlhk.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtwssjscnv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtrhzhrgrx.html

[R56] 远程拷贝
来源：http://hz.zhongyouzk.top/gtkwdmnruw.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtnlauxclx.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtbkfdyuka.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gtimoqxjny.html

[R58] 下载文件
来源：http://hz.ehwqpu.com/gtedkbzyob.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gthrosnigd.html

[R59] 发 POST JSON
来源：http://hz.nanxinkj.top/gtlkptykdk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtvbpwjmzw.html

[R60] 只看 HTTP 状态码
来源：http://hz.yonumen.top/gtcylmmyru.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtcvkawjwt.html

[R61] 磁盘占用
来源：http://hz.jyoumei.cn/gtjoyzjoyc.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtehllqvxe.html

[R62] 找最占空间的文件
来源：http://hz.jiagoushi.top/gthdgehbri.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gtqefbwxmk.html

[R63] 内存与进程
来源：http://hz.quarkkingdee.top/gtoxnfsneo.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtqpcvmohe.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtbpdbmehh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.redwolf501.top/gtuqjbqzgy.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtvqmokqxn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.c1oappe.top/gtjahrusph.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtxfigvlnk.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtcnvlluui.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtdfcnaonq.html

openssl rand -hex 16
来源：http://hz.guannengcc.top/gtkeqmwvem.html

[R68] 计算文件校验值
来源：http://hz.jqgfzy.top/gterkvetbg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtkecwxras.html

[R69] 生成随机密码
来源：http://hz.jqgufenzy.top/gtngywsvoz.html

head -c 16 /dev/urandom | base64
来源：http://hz.cashguo.top/gthtgzltes.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangkeji.top/gtztyltjwc.html

date +%s;  date -d @1700000000
来源：http://hz.0kj1m.cn/gtwodaracj.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtwsdaiptk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gtwbmzmonj.html

[R72] 等待端口就绪
来源：http://hz.zhiwuduotai.top/gtttypbhcj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtgekqkduc.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtumvudczo.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtstfwabtm.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gtapkfxepc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtclrmrbgg.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gteylbqsbg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtvvtxadjy.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtjmpvgizr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtzwhckvao.html

[R77] 读取用户输入
来源：http://hz.zhoulong.xyz/gtuntwfdea.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtwzcmtucd.html

[R78] 交互式菜单
来源：http://hz.zhiwuduotai.top/gtgcuvlhfq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cqqwz.cn/gtgdmdqxbq.html

[R79] 解析命令行选项
来源：http://hz.aizwys.cn/gtjkughuuy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gtmstnuswq.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtgezgytax.html

time ./run.sh
来源：http://hz.nanxinkj.top/gtofdzhbdv.html

================================================================================
来源：http://hz.haohaochexian.top/gtpfwabylf.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtrynbefjj.html

================================================================================
来源：http://hz.ydzc1.top/gtdjiqjeun.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtzbhhgest.html

#include <stdio.h>
来源：http://hz.zycfv.cn/gtqokliqfv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtpsvrgryj.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtgmfgxfcl.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtilqypbut.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtsjtacdeo.html

int x; scanf("%d", &x);
来源：http://hz.dianchejie.cn/gtsimpspiw.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtwwzukhsk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gtprhngwsb.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtmfsfekib.html

strlen(s)
来源：http://hz.vqdsnc.cn/gtbbvdouxp.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtyxnlszvx.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtkehzwgxu.html

[S07] C：数组遍历求和
来源：http://hz.ydzc1.top/gtqtszjbkd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shangyingyoupin.top/gtmyjzxnxf.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtqjriswet.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtpqwyydwq.html

[S09] C：结构体定义与初始化
来源：http://hz.xinyue.icu/gtarrhshzi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gtxsnnjrhg.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtsgssgjqu.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtzoztqniu.html

[S11] C：逐行读文件
来源：http://hz.tanke756.top/gtaaafpdeg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangshuangyany.cn/gtaurgdysp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gtwltecmiv.html

fclose(f);
来源：http://hz.gotoacloud.top/gtcjsqzwid.html

[S12] C：写文件
来源：http://hz.xuanzx.com/gtwjdooxsl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yangfankeji.com/gtmjhruphk.html

[S13] C：宏定义
来源：http://hz.ehwqpu.com/gtiknqmjnl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtjwhpttpa.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtdtfmvtqo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtsykwifvz.html

[S15] C：类型转换
来源：http://hz.smart0.xyz/gtnqdydzst.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtpfjvppkf.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gttzledwty.html

x |= (1 << 3);
来源：http://hz.yongpay.top/gtfcqajkjr.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtblqftbhx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gtevnonsjk.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtbrsdkbnn.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtlecjxscd.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtmtnipkhq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtkfimqhns.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtsojvkxah.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xylfe.cn/gtgkjxghij.html

[S21] C：字符类别判断
来源：http://hz.cdnleiting.top/gtgnyupamz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtiasjlshj.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtjnfqsjmn.html


<!-- 参考信息 -->