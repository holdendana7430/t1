代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shuidangran.top/gtshicqrmd.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangshuangyany.cn/gtmeoaatdy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtbkcttkuu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtcfxrgbme.html

[Q61] 移动平均
来源：http://hz.havefunace.top/gtxydejnhy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.9152youxi.cn/gttiakwend.html

[Q62] 分组占比
来源：http://hz.cashguo.top/gtoodwmwxu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtptdcysfx.html

[Q63] 开启事务
来源：http://hz.shzxlz.cn/gteahdzjxq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.vqdsnc.cn/gtxqnnrzth.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtsgnzusuw.html

COMMIT;
来源：http://hz.redwolf501.top/gtdfiyvrrr.html

[Q65] 回滚事务
来源：http://hz.hongshengwenyu.top/gtrqunckga.html

ROLLBACK;
来源：http://hz.cqqwz.cn/gtdpsrlkxt.html

[Q66] 行锁查询
来源：http://hz.tian-w.cn/gtaeuhwgff.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yongpay.top/gtgkosynbp.html

[Q67] 设置隔离级别
来源：http://hz.mhx1999.top/gtbnfrmeci.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gtlbozgtia.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gtvzswnqrn.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtxvdbmdej.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtrnrxyhuf.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtcnfrvspl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.guannengcc.top/gtwcnmpcls.html

[Q70] 更新统计信息
来源：http://hz.hfpthk.cn/gtctyiniuh.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtvtlfgoqa.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gtcqahlxdv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhiwuduotai.top/gtumsqzvut.html

[Q72] 查看索引
来源：http://hz.yj20258.top/gtoomhsryc.html

SHOW INDEX FROM users;
来源：http://hz.mhx1999.top/gtdwabzjtv.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gthlqmrwvq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtczkwhgsp.html

[Q74] 强制使用索引
来源：http://hz.guannengcc.top/gthymohbfe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtbhhivghl.html

[Q75] 日期格式化
来源：http://hz.shangyingyoupin.top/gtzldmtffm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtkqkjkbuq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gtbnhpdpzr.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gtufsduwgx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuanzhike.top/gtejxwwzoy.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtamkmrfsr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtirwnwvir.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtqlxllihl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtmfsmzqua.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gtymcqqbdj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gthoigfhit.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtdzqdztki.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtjewkhjbr.html

[Q81] 字符串替换
来源：http://hz.daxiang520.top/gtcfixpmlj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pengpengdd.cyou/gtzxoojyan.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtogbxzxaq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtslhumgtz.html

[Q83] 大小写转换
来源：http://hz.shangyingyoupin.top/gtbqpljvsj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtmxfbomvw.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtwtyaondk.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtcxpzfybs.html

[Q85] 数值取整
来源：http://hz.mhx1999.top/gtdyrtbqfd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xingfuxueyuan.xyz/gtonzkwhdr.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtqddasnsf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gtooxavkdh.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtjubmizoc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtvgpllpod.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtuczkbiql.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hysaishi.cn/gtlensaldj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtifmepfth.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtdvyflhrf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuanzx.com/gtsixgfnwu.html

[Q90] 生成序号列
来源：http://hz.c1oappe.top/gtxyofcbdi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuanzx.com/gtvvcbpsvx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtftrndvon.html

R. Bash 专题
来源：http://hz.zhoulong.xyz/gtiyouhlkp.html

================================================================================
来源：http://hz.zdqjudy.top/gtwazmzymr.html

[R01] shebang 与严格模式
来源：http://hz.redwolf501.top/gtjtkurbwa.html

#!/usr/bin/env bash
来源：http://hz.mhx1999.top/gthjbshiqq.html

set -euo pipefail
来源：http://hz.zhoulong.xyz/gtpzmsxysm.html

[R02] 变量赋值与使用
来源：http://hz.ydzc1.top/gtaguuwisl.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtxmujcvfq.html

[R03] 只读变量
来源：http://hz.dashuyun.cn/gthqgfcdda.html

readonly PI=3.14
来源：http://hz.yanxiufei.cn/gtgsncvgxo.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtzxgknmor.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtukhsohns.html

[R05] 参数默认值
来源：http://hz.kuanghao11.cn/gtczanletc.html

name="${1:-default}"
来源：http://hz.tianlin.xyz/gtblsfguqe.html

[R06] 判断命令是否存在
来源：http://hz.guannengcc.top/gtyvydlyqm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtrwbudyfx.html

[R07] if 判断文件
来源：http://hz.cdnleiting.top/gtqnfufyil.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xziqi.cn/gtfziuicbl.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gtowewglze.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtvmdlckoc.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtigzwcsaz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtzuhkbtic.html

[R10] 正则匹配
来源：http://hz.hammf.cn/gtgvdrletl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnxiangtu.top/gtcfdvsekb.html

[R11] case 多分支
来源：http://hz.ydzc1.top/gtdiebukyr.html

case "$1" in
来源：http://hz.gzhubu.top/gtnzryofiy.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtvxkqhaxj.html

stop)  echo "停止" ;;
来源：http://hz.chenzaomai.com/gtcdgzztty.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtvtoxipac.html

esac
来源：http://hz.jqgufenzy.top/gtkwwxfgbj.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtjcntacpe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shangyingyoupin.top/gtkxypmmoi.html

[R13] for 计数循环
来源：http://hz.shanyushiyangkeji.top/gtjiugsgng.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cheryme.top/gttkronahy.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtnkrbvgqt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtsxpkukzf.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtauatwecx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtxbthlqiq.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gtwmbbhomf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jianghu66.top/gtizyxzwap.html

[R17] 数组定义与取值
来源：http://hz.cucudq.cn/gthjvazkpo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gtzhpqyjar.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtzgythfku.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtbdmltqew.html

[R19] 数组长度
来源：http://hz.quarkkingdee.top/gtauvapfne.html

echo "${#arr[@]}"
来源：http://hz.sufxvd.cn/gtjwqbedwc.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtwntdasxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhijiandao.cn/gtdviigxts.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtgrflgjjn.html

echo "${#s}"
来源：http://hz.andypj.xyz/gtacxwdsxt.html

[R22] 截取子串
来源：http://hz.gogol.net.cn/gtvukpdhsf.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtuolplryv.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gtztgjdqsx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxuanxn.top/gtqvgiraxb.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtqlqjwzdr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gthzhqtdix.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gtajbhlmam.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gtudettvpu.html

[R26] 命令替换
来源：http://hz.shanyushiyangkeji.top/gtwpqyqmrt.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtlynxkbuf.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtxgdulbtr.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtrgjvqgxd.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtknxyizpl.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtyqvvwhkk.html

[R29] 定义函数
来源：http://hz.jqgufenzy.top/gtsdfytkhr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gthnvjqnht.html

[R30] 函数返回状态码
来源：http://hz.ivvv.top/gtbybvtryd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj202588.top/gtweuksuah.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtrcsggcbf.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gthscbrnet.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtmdpaqgyb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jyoumei.cn/gtfzxdhmcx.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtyikjmsmb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cqqwz.cn/gtuvwuwfpy.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gtvnzhjlny.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtjfenwdlw.html

[R35] 后台执行并等待
来源：http://hz.dianchejie.cn/gticowkrvh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nanxinkj.top/gtvccnzmvu.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtuwdnwfmg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shzxlz.cn/gtagwtxgem.html

[R37] 把输出赋给变量
来源：http://hz.fzhhl.top/gtdcoshpke.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtitcgppyx.html

[R38] 管道串联
来源：http://hz.pengpengdd.cyou/gtlkxzoscn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtwgotcopr.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtxqzycfzi.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtjyjugdme.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtotndepzc.html

echo "log" >> out.log
来源：http://hz.chenlongwang.top/gtylozohft.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangtech.top/gttgtnclje.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtlemvllae.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtftwpuqdc.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtbnisffih.html

[R43] 按名字查找文件
来源：http://hz.aizwys.cn/gtdimofswq.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtddmnbflh.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtfyylthdv.html

find . -mtime -7 -type f
来源：http://hz.nanxinkj.top/gtqazxlyly.html

[R45] 批量删除
来源：http://hz.chenjidiqi.icu/gtlentuscx.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtjsiycnhz.html

[R46] 递归替换文件内容
来源：http://hz.jianghu66.top/gtstepkbuh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtsmmdodof.html

[R47] sed 单行替换
来源：http://hz.redwolf501.top/gtmfhdyytw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ybcxt.top/gtznknzckt.html

[R48] awk 取指定列
来源：http://hz.andypj.xyz/gtxsgcmrhq.html

awk '{print $1, $3}' a.txt
来源：http://hz.tian-w.cn/gtamtjcawb.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gterivrdpi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtkumkkswg.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtiaaelaur.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtvqokvtql.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtzcvnzcoa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ppjwa.cn/gtfmtzwbvr.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtwrzibrig.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtmnwmtfzd.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtlmvrrcon.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.9152youxi.cn/gthefkocks.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtjnvkgrsm.html

diff a.txt b.txt
来源：http://hz.chenzaomai.com/gtngotfghq.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtnjwgbtia.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ivvv.top/gthfydvuei.html

[R56] 远程拷贝
来源：http://hz.zhixingplan.top/gtnupfajnf.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtgywgnook.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtamueyeqs.html

ssh user@host 'uptime'
来源：http://hz.cheryme.top/gtkabyqtnv.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtvtbuukxp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtskfbczsp.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtbgdnrohp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtwnhxtbux.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuxming.cn/gtfygognsl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.kuanghao11.cn/gtyxtpefjd.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtpmuujjvf.html

df -h;  du -sh *
来源：http://hz.pycfn.com/gteprxzauz.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtbpdjrmke.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtnhabdoin.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtbcjfaltl.html

free -h;  ps aux | grep nginx
来源：http://hz.aibaodan.cn/gtsceiobue.html

[R64] 结束进程
来源：http://hz.smart0.xyz/gtsifjbhzh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtsgstacej.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtcihfpmhn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jiagoushi.top/gtkvsoxcey.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gtojriqjtf.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtjhkqqpia.html

[R67] 生成随机十六进制串
来源：http://hz.shangyingyoupin.top/gtlkkgcbgc.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtxmqpdwzp.html

[R68] 计算文件校验值
来源：http://hz.feifeiyinyue.top/gtbakauiwj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuanzx.com/gtcmzrzloq.html

[R69] 生成随机密码
来源：http://hz.xinyue.icu/gtfxvvixax.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtribrohha.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtvqfebvtq.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtwdjzqphf.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtosvuloyc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ivvv.top/gtwhfkvniq.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gttjmbmsbb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yongpay.top/gtdebtahhc.html

[R73] 分割大日志
来源：http://hz.shzxlz.cn/gtkhimfyzn.html

split -l 1000 big.log part_
来源：http://hz.ywan-chungtsiang.top/gtdtyqzhbp.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gtsxhshwvt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtjqbkwtuy.html

[R75] 导出环境变量
来源：http://hz.jiagoushi.top/gtpurscyoo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.meibo888.top/gtleqzteon.html

[R76] 使用临时文件
来源：http://hz.c1oappe.top/gtuyoynusv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtmkbxdgsp.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtrcnphktm.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtdswaedie.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtivnertex.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtoxvytsar.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtokfnglmk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gthfdefwiy.html

[R80] 查看脚本执行耗时
来源：http://hz.hywenlv.cn/gttrnfhldl.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtlpfniile.html

================================================================================
来源：http://hz.yvedp.cn/gtdteqnitw.html

S. C / C++ 专题
来源：http://hz.yueranfly.top/gtwuvlleoz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnflwpqpg.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtkhlyqzfb.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gtattvrdpz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtimymihnw.html

[S02] C：变量与格式化输出
来源：http://hz.yongpay.top/gtrqoeyzbk.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtijnoehtw.html

[S03] C：读入整数
来源：http://hz.chenzaomai.com/gtwgafaecg.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtulbdahsz.html

[S04] C：字符串复制
来源：http://hz.yuanzhike.top/gtzksbqvvn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuetiantiany.cn/gtjtolsowu.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtvqqejlfb.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtxtufdayq.html

[S06] C：字符串比较
来源：http://hz.kuanghao11.cn/gtycbzstrq.html

strcmp(a, b) == 0
来源：http://hz.yangfankeji.com/gtzokwrdte.html

[S07] C：数组遍历求和
来源：http://hz.chenlongwang.top/gttbknbwvt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtkhnozjta.html

[S08] C：动态内存分配与释放
来源：http://hz.cucudq.cn/gthwqoaugg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhoulong.xyz/gtjshtpfza.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gtrxorxkue.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cucudq.cn/gtjjcwfrlv.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtrxnseplg.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtavclxunx.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtadsglhtn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gtqzckktjo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuetiantiany.cn/gtngiejrvx.html

fclose(f);
来源：http://hz.feifeiyinyue.top/gtvywwdkih.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtxhkvrapr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.feifeiyinyue.top/gtlfppiecx.html

[S13] C：宏定义
来源：http://hz.meibo888.top/gtiacxqehq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtkqzwefpe.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtgfzssccj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtcycnsvcg.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtzjtrrmvz.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtckevugmh.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtbakajgdf.html

x |= (1 << 3);
来源：http://hz.cucudq.cn/gthlejateg.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gtedwuibzd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhiwuduotai.top/gtaqccujga.html

[S18] C：命令行参数
来源：http://hz.gotoacloud.top/gtcpwepyku.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtipijkzij.html

[S19] C：快速排序
来源：http://hz.quarkkingdee.top/gtjkswodiv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtixrydbmx.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtlskdziwk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtdxrkrqhp.html

[S21] C：字符类别判断
来源：http://hz.jinqigfzy.top/gtvhtphgpr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gtycbhtufu.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtepfqozdy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gtkcxvarmm.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtbuyxtvgf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hammf.cn/gtjyqpwclu.html

[S24] C：获取本地时间
来源：http://hz.feifeiyinyue.top/gtbmeubxda.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gthrqksqxe.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtkeibrxpy.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtaojbfbem.html

[S26] C：内存清零
来源：http://hz.yj20258888.top/gtipkevyzr.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtukuewzqg.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtcgkfmxbp.html

const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtjdflmeit.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtdwesqxdp.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtpvublckk.html

[S29] C：变参函数
来源：http://hz.feifeiyinyue.top/gtkovqmnen.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.dashuyun.cn/gtwadbrbaa.html

[S30] C：头文件保护
来源：http://hz.quarkkingdee.top/gttjipoesh.html


<!-- 参考信息 -->