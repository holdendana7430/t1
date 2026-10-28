代发 wailian999

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtvffeiofx.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtigxqooqw.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtjaddhdyw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuanzx.com/gtwdewcczy.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtkctlxzqs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gthyqczuyq.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtvtfafjmr.html

SAVEPOINT sp1;
来源：http://hz.yongpay.top/gtqvxiyrqy.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gtsdgmfnmk.html

[Q69] 查看执行计划
来源：http://hz.tianlin.xyz/gtunxvqczp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtcilhqztg.html

[Q70] 更新统计信息
来源：http://hz.xinyue.icu/gtaosjcppi.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gtczlrzczj.html

[Q71] 查看建表语句
来源：http://hz.jinghuilouyu.cn/gthhlytmmt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hongshengwenyu.top/gtdphvdctj.html

[Q72] 查看索引
来源：http://hz.shangyingyoupin.top/gtcepszzdx.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtcmwebxjg.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtiesbjpmd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtfbdeyago.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtfnsoxazx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtetpnuuki.html

[Q75] 日期格式化
来源：http://hz.shuidangran.top/gtpvtrgjfj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtbqwthdod.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtsqzqaryo.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtdlfcwiyh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.bjfxy.top/gtxzvqrpai.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtuoxbmorz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtlvdfybno.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtdptiingw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtbcldidpe.html

[Q79] 字符串拼接
来源：http://hz.c1oappe.top/gtcnafiumi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinyuanbaomall.cn/gtjzjjszpj.html

[Q80] 字符串截取
来源：http://hz.jiagoushi.top/gtdnlryzpd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtbnqpikqi.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtiychwnkf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zycfv.cn/gtrimugsaq.html

[Q82] 字符长度与字节长度
来源：http://hz.xuetiantiany.cn/gtuveuvaix.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gthgdosalc.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtchkeblyf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gtjhfgqwqu.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtdjdoxukz.html

SELECT TRIM(name) FROM users;
来源：http://hz.gotoacloud.top/gtcvekoxpo.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtrkqsubuq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtxxexjewr.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtmjtwqkdd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtnlqbhmsm.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtgmchxtmc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinyuanbaomall.cn/gtnxopoxtd.html

[Q88] 行转列（条件聚合）
来源：http://hz.haohaochexian.top/gtumlbefss.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtabfpadaq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangkeji.top/gtqfsjnyiv.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gthfsqmcgc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shuidangran.top/gtfkjopoyo.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gthbiutxhb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hfpthk.cn/gthjihenzt.html

================================================================================
来源：http://hz.yj202588.top/gtqunrecnl.html

R. Bash 专题
来源：http://hz.kuanghao11.cn/gtzxxuxpew.html

================================================================================
来源：http://hz.sysykeji.top/gtobwvsjca.html

[R01] shebang 与严格模式
来源：http://hz.c1oappe.top/gtqrxjqmbn.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtrbvnekqz.html

set -euo pipefail
来源：http://hz.zycfv.cn/gtjsqpmuyr.html

[R02] 变量赋值与使用
来源：http://hz.ivvv.top/gtgodryrov.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtebxaxgkx.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtdroecfvy.html

readonly PI=3.14
来源：http://hz.yonumen.top/gtyplnegiz.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gtdiikihjz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtiwjzkthb.html

[R05] 参数默认值
来源：http://hz.hfpthk.cn/gtezktzyzf.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gtrxzeindh.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtvuznagco.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gtiddzapmu.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gtlkfxvnei.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtjzgodciw.html

[R08] 数值比较
来源：http://hz.zhengqikj.top/gtugmrrfqp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gttdjwdkny.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtwpfhtitv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hywenlv.cn/gtktlagaad.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gtqugdxbrz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jlsjyb.cn/gtfmsounyr.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtvkkrijkf.html

case "$1" in
来源：http://hz.sysykeji.top/gtptneldmq.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtdtqmgfgz.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtlntqjddx.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gtrzhdhwvb.html

esac
来源：http://hz.sysykeji.top/gtamefdfgy.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtmgpagzud.html

for f in *.txt; do echo "$f"; done
来源：http://hz.snrcjt.cn/gtbvwnfiha.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtcxxnlxjv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shzxlz.cn/gtxrdawqgi.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtizxzijeq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuanzhike.top/gtkboyktre.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtjgeuidaz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nwbrower.top/gtjwqkcwul.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtuzbeprhe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtwdqpuibp.html

[R17] 数组定义与取值
来源：http://hz.zycfv.cn/gtrksnosvf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtuzeldamh.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtjaywhdwi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.bjfxy.top/gtarxrseis.html

[R19] 数组长度
来源：http://hz.havefunace.top/gtplrvrcio.html

echo "${#arr[@]}"
来源：http://hz.jinghuilouyu.cn/gtfumcubrd.html

[R20] 关联数组（字典）
来源：http://hz.hammf.cn/gtjwlskzmz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jqgfzy.top/gtywobgudf.html

[R21] 字符串长度
来源：http://hz.jinghuilouyu.cn/gtmcjinzhf.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtwoefsvwj.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtjbpkjzkd.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtgcaudpvx.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtyfxydjet.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhengqikj.top/gttmqbothz.html

[R24] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtmucnipql.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gttlvnuwtp.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gthkojnoqy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtmtwdpxem.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtpbxwdpia.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gtgttgxpbx.html

[R27] 算术展开
来源：http://hz.havefunace.top/gtsscmjoxq.html

echo $((1 + 2 * 3))
来源：http://hz.aibaodan.cn/gtzackutgt.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gttwoeskzr.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gttllizugh.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtuyevdjna.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtthiqqrky.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtgxarjoxs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yanxiufei.cn/gtvjwjwjjf.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtecsvmjiz.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtueacnlre.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtjatlqubi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gtezjwmrsy.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtuasdiguq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtxvuoaoea.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gteidzlarc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtvjhajsex.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gteprurior.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gticpgkhrm.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gtwiardwqj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinghuilouyu.cn/gtbwwxgtni.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtgynpcdxp.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtrtfjsrpj.html

[R38] 管道串联
来源：http://hz.316326.xyz/gtatiftlau.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shzxlz.cn/gtijrztgdg.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtskaksumv.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtxbvpdlvt.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtrtklsmvh.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtvuwudlul.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtofasnkai.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtsykbiiyj.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gttvjntsco.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtyxkgltxe.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtkyjekmhf.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtlywrlyoz.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gtmwvxxdka.html

find . -mtime -7 -type f
来源：http://hz.chenzaomai.com/gtmxrftwnx.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtdoriwlzt.html

find . -name "*.tmp" -delete
来源：http://hz.tian-w.cn/gtqqoibfys.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtnsfczifw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtbepxtvez.html

[R47] sed 单行替换
来源：http://hz.zhoulong.xyz/gtbmbbvwuh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtksiisvyv.html

[R48] awk 取指定列
来源：http://hz.shzxlz.cn/gtvzsauvwe.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtnnaidyuf.html

[R49] awk 带条件
来源：http://hz.xinyue.icu/gttppgsbra.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenjidiqi.icu/gtuzxkeftm.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtvcwydslj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gteprlvnac.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtckuqgvju.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.bjfxy.top/gtnteytick.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtvgzcbhvm.html

wc -l a.txt
来源：http://hz.gogol.net.cn/gtymfziquk.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtiegpezru.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.quarkkingdee.top/gtsslykrbp.html

[R54] 比较两个文件
来源：http://hz.wangshuangyany.cn/gtmxtlrnpe.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtlirxpbmi.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtsmhyvllr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtkuavzmgu.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtgnzycwld.html

scp file user@host:/path/
来源：http://hz.sufxvd.cn/gtddvufmcb.html

[R57] 远程执行命令
来源：http://hz.yueranfly.top/gtkxwqbzcz.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gtlwkknkjm.html

[R58] 下载文件
来源：http://hz.jianghu66.top/gtvvhempab.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtmmfxtjvh.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gtfbxrplxa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtqnwssqmc.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenzaomai.com/gtvisfiops.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhongyouzk.top/gthbqskhss.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtfwxvwexi.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtawlyfekz.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gthykwgvgn.html

du -ah . | sort -rh | head -10
来源：http://hz.hammf.cn/gtapzeazeb.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtaqtyxjsw.html

free -h;  ps aux | grep nginx
来源：http://hz.ydjk.org.cn/gtnxcnjotv.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtykzzdobx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.iojbl.cn/gtaykqlphr.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtpzbshkel.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinyuanbaomall.cn/gtkquerbnv.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtgyuamyhj.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtxyxazlhg.html

[R67] 生成随机十六进制串
来源：http://hz.xinyue.icu/gtalnayevx.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gtnkztfhih.html

[R68] 计算文件校验值
来源：http://hz.wangshuangyany.cn/gtwktrrhde.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinghuilouyu.cn/gtyerbbthu.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangkeji.top/gtpnwayvds.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gtqrirhyih.html

[R70] 时间戳与互转
来源：http://hz.redwolf501.top/gtwevwviij.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gtdklenfoa.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtasujkpdl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gthaekbjui.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtrhrmgdif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtysffkalm.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtnnmisdua.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtixkffyov.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gtofugslci.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gthjbhitqy.html

[R75] 导出环境变量
来源：http://hz.xingfuxueyuan.xyz/gtedelnllr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gtujrhgfba.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtpoqkeoqj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtjqmgubuo.html

[R77] 读取用户输入
来源：http://hz.jiagoushi.top/gtojxijjhu.html

read -rp "请输入: " ans
来源：http://hz.ydzc1.top/gttoznklhj.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtiqadskil.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtjrskictq.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gthlldqesb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dianchejie.cn/gtedkeyeyi.html

[R80] 查看脚本执行耗时
来源：http://hz.jinyuanbaomall.cn/gtnzqptzua.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtkwhhtkba.html

================================================================================
来源：http://hz.hysaishi.cn/gtudwhosmx.html

S. C / C++ 专题
来源：http://hz.hongshengwenyu.top/gtattfysnm.html

================================================================================
来源：http://hz.daria6918.cn/gthljcldvj.html

[S01] C：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtfonkqhdk.html

#include <stdio.h>
来源：http://hz.ppjwa.cn/gtrrafxcyy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtolttfhle.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gthzplnoov.html

int a = 10; printf("%d\n", a);
来源：http://hz.cqqwz.cn/gtychqwdzb.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtmsadzdkt.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtrppugddd.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gthbxfwntg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtakldqhbx.html

[S05] C：字符串长度
来源：http://hz.hongshengwenyu.top/gtuvshbfvq.html

strlen(s)
来源：http://hz.jqgfzy.top/gtnernmbrx.html

[S06] C：字符串比较
来源：http://hz.jqgfzy.top/gtqfqzmbiu.html

strcmp(a, b) == 0
来源：http://hz.nanxinkj.top/gtluedipdm.html

[S07] C：数组遍历求和
来源：http://hz.shangyingyoupin.top/gtjkvyuwhe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daria6918.cn/gtfwqyfzdc.html

[S08] C：动态内存分配与释放
来源：http://hz.yongpay.top/gtbogmxfnx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cdnleiting.top/gtqqbviagk.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtouinlfhh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sxryk.cn/gtaodbtjqo.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gtymmjwppv.html

int *p = &a;  *p = 5;
来源：http://hz.iojbl.cn/gtzqoowlts.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtcrqvuscq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gthgqkuhnn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtmurcpqcm.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtqwjuyvbn.html

[S12] C：写文件
来源：http://hz.smart0.xyz/gtdowajgue.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtkdajbpev.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtpdxekuds.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtrivecxmh.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtcethukce.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tian-w.cn/gtgytjvfcv.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtuixbhyni.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtbfdvqvwv.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtldyuwbwe.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtcdckzcag.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtvuejvaef.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtkjymnseh.html

[S18] C：命令行参数
来源：http://hz.andypj.xyz/gtwnxrsxgn.html

int main(int argc, char **argv)
来源：http://hz.nanxuanxn.top/gtfurerrve.html

[S19] C：快速排序
来源：http://hz.zhengqikj.top/gtfyzakjce.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gthvkeyvqe.html

[S20] C：二分查找
来源：http://hz.chenzaomai.com/gtfovjkdzl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtmopgtbjc.html

[S21] C：字符类别判断
来源：http://hz.52xcode.cn/gtyybhngcm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtktuaxlsv.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gtslvgjhzb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtmlhxqlwm.html

[S23] C：随机数
来源：http://hz.shanyushiyangtech.top/gtltiywlds.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.feifeiyinyue.top/gtuwyvlcfu.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtidywgatl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnxiangtu.top/gtgasmdywl.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gttvwyixaa.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtotjyjouc.html

[S26] C：内存清零
来源：http://hz.meibo888.top/gtkqdgkyxg.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtybipzfeu.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtcydgrccd.html

const double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtdvvjnnba.html

[S28] C：静态变量
来源：http://hz.wangdashe.top/gtwwtfcssj.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtslufsrqb.html

[S29] C：变参函数
来源：http://hz.xylfe.cn/gtpxtpcxas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtmdqfaexr.html

[S30] C：头文件保护
来源：http://hz.nanxuanxn.top/gtlusmwyip.html

#ifndef X_H
来源：http://hz.meibo888.top/gtpsnhzrnd.html

#define X_H
来源：http://hz.316326.xyz/gttnawjjtb.html

#endif
来源：http://hz.pycfn.com/gtkictdwdj.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtctvxbues.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtygslubed.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtckjllkjf.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gtgfqmlhhw.html

std::string s = "hi";  s += "!";
来源：http://hz.ydjk.org.cn/gtdhnjxhbn.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtkhuwgrmh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gzhubu.top/gtxugcbtgu.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtyvzxthpy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtlqmzyrbb.html


<!-- 参考信息 -->