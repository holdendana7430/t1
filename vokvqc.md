代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.jianghu66.top/gtfiqeqkre.html

[Q69] 查看执行计划
来源：http://hz.xziqi.cn/gtxyghdtjy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gtihbwpaew.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtgxhdkxxd.html

ANALYZE TABLE users;
来源：http://hz.redwolf501.top/gtgpkgaefu.html

[Q71] 查看建表语句
来源：http://hz.yanxiufei.cn/gtvygfejub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhixingplan.top/gtfotfkzbm.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gtxmeqllet.html

SHOW INDEX FROM users;
来源：http://hz.redwolf501.top/gtnhebfjvs.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gtkppjpoou.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gtvfqtbfeu.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtgxukalvz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtvahowjmg.html

[Q75] 日期格式化
来源：http://hz.yuxming.cn/gtfgshilil.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtvawosgbc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.meibo888.top/gthzluiqeh.html

[Q76] 按天统计
来源：http://hz.sxryk.cn/gttypkuuxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shuidangran.top/gtbfgoahmi.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gtdsdhrwfi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xingfuxueyuan.xyz/gtuwfxfgvt.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtlkhtwdpg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gthberqndn.html

[Q79] 字符串拼接
来源：http://hz.sweek.top/gtbyikrwjd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhongyouzk.top/gtdbfgdrtf.html

[Q80] 字符串截取
来源：http://hz.yvedp.cn/gtmaobckqf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtgpymbwna.html

[Q81] 字符串替换
来源：http://hz.haohaochexian.top/gtyifcgpvm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sweek.top/gtlbhswpln.html

[Q82] 字符长度与字节长度
来源：http://hz.ydjk.org.cn/gtlahldssg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtxrfxutep.html

[Q83] 大小写转换
来源：http://hz.9152youxi.cn/gtpotxnxdm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gzhubu.top/gtrzeqygpc.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtrjbpodfw.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258.top/gtubaahizx.html

[Q85] 数值取整
来源：http://hz.yuanzhike.top/gtugnriwfk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gzhubu.top/gtvssxkhhs.html

[Q86] 读取 JSON 字段
来源：http://hz.tianlin.xyz/gtsyzoihjl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtouiemzky.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtyfogwfxb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtnyakwhte.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj202588.top/gtchdmefpd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtuehxcbis.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhixingplan.top/gtktdijgwq.html

[Q89] 判断表是否存在
来源：http://hz.gaohongyu789.top/gtagirrguk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtmjsmhuns.html

[Q90] 生成序号列
来源：http://hz.cashguo.top/gtqlrnznjz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtuvygwpkd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqmhyoxyg.html

R. Bash 专题
来源：http://hz.gzhubu.top/gtpbfvorct.html

================================================================================
来源：http://hz.316326.xyz/gtwfcvtzab.html

[R01] shebang 与严格模式
来源：http://hz.yj20258888.top/gtfrocliwb.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtisbdjuzn.html

set -euo pipefail
来源：http://hz.sweek.top/gttudjpzbj.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gttkwcczfz.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtkytmmtdu.html

[R03] 只读变量
来源：http://hz.kuanghao11.cn/gtgznupkwd.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtcrymhtql.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtzrkoyjai.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtdakhdvfu.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtnubwjdzr.html

name="${1:-default}"
来源：http://hz.xuetiantiany.cn/gtcjcpvmat.html

[R06] 判断命令是否存在
来源：http://hz.xingfuxueyuan.xyz/gttktyucfn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtsyqnkqad.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gtherorbcl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gttnszkrve.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtltugrwih.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtqwvlhbco.html

[R09] 字符串比较
来源：http://hz.hnxiangtu.top/gtscntcbys.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtuoiiksxe.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtzoxoppwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.quarkkingdee.top/gthjtpwdzw.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtbravfntf.html

case "$1" in
来源：http://hz.cdnleiting.top/gtpecbhffd.html

start) echo "启动" ;;
来源：http://hz.jqgufenzy.top/gtahxztikb.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gteuxysfld.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtnpgteogp.html

esac
来源：http://hz.shangyingyoupin.top/gtqbabtkch.html

[R12] for 遍历文件
来源：http://hz.cqqwz.cn/gtnpmwdnkp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnqzz.top/gtfdnjxfxq.html

[R13] for 计数循环
来源：http://hz.gogol.net.cn/gtifokfxyr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yonumen.top/gtquuyonhz.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtpnqjdmgt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nwbrower.top/gtvdkgcmla.html

[R15] while 逐行读文件
来源：http://hz.zhijiandao.cn/gtduiffmes.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtugxslvuk.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtgzzzcsbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gtdzposiwv.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtrcczrjsx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jyoumei.cn/gtwdgdgjoq.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtxswgtteu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhongyouzk.top/gtgutllycu.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtexggggdv.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtjksuwnlh.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangtech.top/gtqmqitvla.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtoygnayvu.html

[R21] 字符串长度
来源：http://hz.shangyingyoupin.top/gtjvkuiabt.html

echo "${#s}"
来源：http://hz.sweek.top/gteiconike.html

[R22] 截取子串
来源：http://hz.52xcode.cn/gtpsopikza.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtzkngtzrv.html

[R23] 字符串替换
来源：http://hz.zdqjudy.top/gtzuzbknvk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtdfxcsqmz.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtsuwrnrlh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yuanzhike.top/gtmggjljcf.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtwahxgciz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gtlgigqlnd.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtpxasqonx.html

now=$(date +%F); echo "$now"
来源：http://hz.yanxiufei.cn/gtozjncqtl.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtdzjekhsu.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtcppkjmza.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtvzawjhhn.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtlzlxdrul.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtpxbencsi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hammf.cn/gtapsfbytv.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gthlglwnlu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtwnzoszdm.html

[R31] 局部变量
来源：http://hz.cdnleiting.top/gtmjpppqio.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhiwuduotai.top/gtxlrblzmy.html

[R32] 参数个数校验
来源：http://hz.chenzaomai.com/gtvcosdujj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtknovzgbl.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtpqqlvvhr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtrsfidpsv.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtijfgnrct.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtwaetasmu.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtgurvumjc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtewyvfsrq.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtrpaguyeo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtqgrfmzqc.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gtkfzhstik.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtinqhqtph.html

[R38] 管道串联
来源：http://hz.guannengcc.top/gtyjegabia.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jiagoushi.top/gtgxkefbea.html

[R39] 重定向标准输出与错误
来源：http://hz.shzxlz.cn/gtklelzjlg.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtlwhtbzmu.html

[R40] 追加写日志
来源：http://hz.tian-w.cn/gtdsjfnenz.html

echo "log" >> out.log
来源：http://hz.ppjwa.cn/gtjdkcuecs.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtknphcrfg.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangtech.top/gtlatsbdty.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtrfkbyfhp.html

wc -l < a.txt
来源：http://hz.zhongyouzk.top/gtcrultahb.html

[R43] 按名字查找文件
来源：http://hz.xylfe.cn/gtcxghgkdj.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtaspyqqgn.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtqajzfsgw.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtsqsvzpih.html

[R45] 批量删除
来源：http://hz.shanyushiyangtech.top/gtrfmascuj.html

find . -name "*.tmp" -delete
来源：http://hz.hammf.cn/gtmbeqnwwb.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtrtyqwedq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuanzhike.top/gtubyywiah.html

[R47] sed 单行替换
来源：http://hz.xylfe.cn/gtlcwkgajh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtsnchnvfp.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtkyuppzfx.html

awk '{print $1, $3}' a.txt
来源：http://hz.quarkkingdee.top/gtdlngulqh.html

[R49] awk 带条件
来源：http://hz.ehwqpu.com/gtlyuiopuf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnxiangtu.top/gtqlbvtqaj.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtixqfitok.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtnmtwjcnt.html

[R51] 排序去重取前几
来源：http://hz.daria6918.cn/gtzrmlgefd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtbuzdakdo.html

[R52] 统计行数
来源：http://hz.sufxvd.cn/gtfbpziren.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtpoqzgfss.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtcteynprz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtdtwuwywo.html

[R54] 比较两个文件
来源：http://hz.cheryme.top/gtmagafhip.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gtygxatfkb.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtnupvfjjo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gticnfmrya.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtzqrnztsh.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gtqrjzgolc.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtmwkozpvy.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtmmyjjdxg.html

[R58] 下载文件
来源：http://hz.yj20258888.top/gtxxzapfjb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.mhx1999.top/gtyvuepaaf.html

[R59] 发 POST JSON
来源：http://hz.nanxuanxn.top/gtjvpzynsd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jqgufenzy.top/gtlgatznkg.html

[R60] 只看 HTTP 状态码
来源：http://hz.0kj1m.cn/gthgbfovar.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtoudliuxs.html

[R61] 磁盘占用
来源：http://hz.smart0.xyz/gtagdpfehc.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtszgmugpz.html

[R62] 找最占空间的文件
来源：http://hz.zhengqikj.top/gtoxuqolel.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtxzbfhhlf.html

[R63] 内存与进程
来源：http://hz.yangfankeji.com/gtanhprqtb.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtbybtkzgy.html

[R64] 结束进程
来源：http://hz.chenlongwang.top/gtjawzatdp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtyixshmdt.html

[R65] 查看端口占用
来源：http://hz.wangdashe.top/gtkvzypkjc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtkcgpwonj.html

[R66] 定时任务
来源：http://hz.guannengcc.top/gtdwtknjkt.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtbixunokp.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtfxbbchae.html

openssl rand -hex 16
来源：http://hz.wangshuangyany.cn/gtlsepbcjk.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtiqzuhxjp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guowangkeji.top/gtwemfuuxe.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtrzxkfevq.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gtjdupezsm.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gturonnakr.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtzgfvurvz.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtqozovtvx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sxryk.cn/gtovdhsunm.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtmgiakpxv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gogol.net.cn/gtumkiwkeq.html

[R73] 分割大日志
来源：http://hz.xinyue.icu/gtoyjenrmb.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtzanblvul.html

[R74] 批量重命名
来源：http://hz.yvedp.cn/gtuscazvzb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yanxiufei.cn/gttxrnntjk.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtiobvzftw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtcmfkoyxn.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtclamoyez.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtserzyexs.html

[R77] 读取用户输入
来源：http://hz.smart0.xyz/gtabwkoepi.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gtyezohugm.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangkeji.top/gtadtjqstb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtlnrwaswf.html

[R79] 解析命令行选项
来源：http://hz.jinyuanbaomall.cn/gtdpvrvcps.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ivvv.top/gtpwplvmuk.html

[R80] 查看脚本执行耗时
来源：http://hz.pengpengdd.cyou/gtpygctqfk.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtwihejqys.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwfrmcsoy.html

S. C / C++ 专题
来源：http://hz.yj20258888.top/gtctwwmuqj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtlwugfytf.html

[S01] C：Hello World
来源：http://hz.yuanzhike.top/gtqrzhikza.html

#include <stdio.h>
来源：http://hz.gogol.net.cn/gtkmwfmeaf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtdfvjhaxq.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtjysgjamn.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtitppmazn.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtvgocdhga.html

int x; scanf("%d", &x);
来源：http://hz.zhijiandao.cn/gtxqrliozn.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtspbfvsdt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yueranfly.top/gtuqrizdsd.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtudnvkqez.html

strlen(s)
来源：http://hz.smart0.xyz/gtqdqceund.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gtzlzikoes.html

strcmp(a, b) == 0
来源：http://hz.svipenyu.cn/gtotxfkgmf.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gtlqjvetyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtmaxbykgq.html

[S08] C：动态内存分配与释放
来源：http://hz.316326.xyz/gtlmqhreub.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.smart0.xyz/gtiskwznfx.html

[S09] C：结构体定义与初始化
来源：http://hz.hfpthk.cn/gtqfpzsvzx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtexkqeqhp.html

[S10] C：指针与解引用
来源：http://hz.yonumen.top/gtokxhjuck.html

int *p = &a;  *p = 5;
来源：http://hz.zhiwuduotai.top/gtmyzqjuop.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtcoetebuh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtgxgomppo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.mhx1999.top/gthbfdaehl.html

fclose(f);
来源：http://hz.52xcode.cn/gtfayxuiqo.html

[S12] C：写文件
来源：http://hz.yj202588.top/gtmpqyzvee.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gtwhjkxbbt.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtcqpkojwi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dashuyun.cn/gtzwvlwrpo.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtaegprypi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gthkpenuuv.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gtppbjrcuv.html

(double) a / b
来源：http://hz.redwolf501.top/gtfkjzxvxr.html

[S16] C：位操作置位
来源：http://hz.haohaochexian.top/gtwuhxnctn.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtmlfimxzh.html

[S17] C：安全拼接字符串
来源：http://hz.zdqjudy.top/gtedsiwirg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gotoacloud.top/gtdepvcoao.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtlouopfpn.html

int main(int argc, char **argv)
来源：http://hz.havefunace.top/gttdfcpely.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtkivopdaa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtjggxxmow.html

[S20] C：二分查找
来源：http://hz.yongpay.top/gtygpsqnzm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtewfvzbup.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtkccbapwr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yangfankeji.com/gtrjquimne.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtqzyfcqvg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgfzy.top/gtdbxngcmj.html

[S23] C：随机数
来源：http://hz.dashuyun.cn/gtsgsvnwwz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtwhaflzbd.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtlqklmyrz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtpkgfytjl.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtknbmonzm.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtqiozecln.html

[S26] C：内存清零
来源：http://hz.jinyuanbaomall.cn/gtcaaqftyr.html

memset(a, 0, sizeof a);
来源：http://hz.tian-w.cn/gtwrplrwzt.html

[S27] C：定义常量
来源：http://hz.sxryk.cn/gtuvdsrsod.html

const double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtcrmaltin.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtzvvtasdb.html

static int counter = 0;
来源：http://hz.sweek.top/gtkfmgbfca.html

[S29] C：变参函数
来源：http://hz.hywenlv.cn/gtlslkpzra.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtjbwshunt.html

[S30] C：头文件保护
来源：http://hz.redwolf501.top/gthbfmetsy.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtjaaqqiku.html

#define X_H
来源：http://hz.haohaochexian.top/gtonyhdbtb.html

#endif
来源：http://hz.zhongyouzk.top/gtzprahbqv.html

[S31] C++：Hello World
来源：http://hz.yanxiufei.cn/gtshpapsyg.html

#include <iostream>
来源：http://hz.gogol.net.cn/gtielohovj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtoffoxspx.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtxxicrffz.html

std::string s = "hi";  s += "!";
来源：http://hz.dianchejie.cn/gtuypsllnt.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtplkhkgwa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgufenzy.top/gtjoxtmvro.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtuwibajrf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtrxamvaip.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtesymgdus.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtroxgniqx.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtrtzjevpm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtbzjlbtlm.html

[S37] C++：set
来源：http://hz.zycfv.cn/gtjqbavlow.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtezqignjn.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtbzmctltf.html

std::sort(v.begin(), v.end());
来源：http://hz.jinghuilouyu.cn/gtpinufant.html


<!-- 参考信息 -->